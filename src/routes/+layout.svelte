<script>
  import "@skeletonlabs/skeleton/themes/theme-crimson.css";
  import "@skeletonlabs/skeleton/styles/skeleton.css";
  import "../app.postcss";
  import 'iconify-icon';
  import Navbar from "$lib/components/navbar.svelte";
  import Main from "$lib/components/main.svelte";

</script>

<div class="min-h-screen md:pb-16 w-full">

  <slot />

</div>

<style>
</style>
