<script>
  import "@skeletonlabs/skeleton/themes/theme-crimson.css";
  import "@skeletonlabs/skeleton/styles/skeleton.css";
  import "../app.postcss";
  import "iconify-icon";
  import { LightSwitch } from "@skeletonlabs/skeleton";
  import Navbar from "$lib/components/navbar.svelte";
  import SideNav from "$lib/components/sideNav.svelte";
  import Footer from "$lib/components/footer.svelte";
  import Menu from "$lib/components/menu.svelte";
  import Navbar2 from "$lib/components/navbar2.svelte";
  import { fly } from "svelte/transition";

  export let data;
</script>

<svelte:head>
  <title>Jorge Corzo - Portfolio</title>
  <meta
    name="description"
    content="Jorge Corzo portfolio web developer in Australia."
  />
</svelte:head>

<!-- Interface Desktop view -->
<div class="hidden lg:block px-6">
  <div class="flex pt-5 justify-end"><LightSwitch /></div>
  <Navbar />
  <div class="flex gap-4 items-start">
    <div class="lg:sticky lg:top-48">
      <SideNav />
    </div>
    {#key data.url}
      <div
        class=" bg-surface-200 dark:bg-black rounded-2xl"
        in:fly={{ x: 200, duration: 300, delay: 500 }}
        out:fly={{ x: 200, duration: 500 }}
      >
        <slot />
        <Footer />
      </div>
    {/key}
  </div>
</div>
<!-- Interface mobile view -->
<div class="lg:hidden">
  <Menu />
  {#key data.url}
    <div class="mt-12"
      in:fly={{ x: -200, duration: 300, delay: 500 }}
      out:fly={{ x: 200, duration: 500 }}
    >
      <slot />
    </div>
  {/key}
  <Footer />
</div>
