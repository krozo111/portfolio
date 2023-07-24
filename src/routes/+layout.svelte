<script>
  import "@skeletonlabs/skeleton/themes/theme-crimson.css";
  import "@skeletonlabs/skeleton/styles/skeleton.css";
  import "../app.postcss";
  import "iconify-icon";
  import Navbar from "$lib/components/navbar.svelte";
  import SideNav from "$lib/components/sideNav.svelte";
  import Footer from "$lib/components/footer.svelte";
  import Menu from "$lib/components/menu.svelte";
</script>

<svelte:head>
  <title>Jorge Corzo - Portfolio</title>
</svelte:head>

<!-- Interface Desktop view -->
<div class="hidden lg:block px-6">
  <div class="container grid grid-cols-12 gap-10 justify-between mt-[220px]">
    <SideNav />
    <div class="col-span-12 lg:col-span-8">
      <Navbar />
      <div class="bg-surface-700 rounded-2xl">
        <slot />
        <Footer />
      </div>
    </div>
  </div>
</div>

<!-- Interface mobile view -->
<div class="lg:hidden">
  <div class="w-full flex justify-between px-4">... <Menu /></div>
  <SideNav />
  <slot />
  <Footer />
</div>
