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
  <div class="flex pt-5 justify-end sticky top-0"><LightSwitch /></div>
  <div class="container grid grid-cols-12 gap-10 justify-between mt-[180px]">
    <SideNav />
    <div class="col-span-12 lg:col-span-8">
      <Navbar />
      <div class="bg-surface-200 dark:bg-black rounded-2xl">
        <slot />
        <Footer />
      </div>
    </div>
  </div>
</div>

<!-- Interface mobile view -->
<div class="lg:hidden">
  <Menu />
  <slot />
  <Footer />
</div>
