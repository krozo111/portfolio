<script>
  import "@skeletonlabs/skeleton/themes/theme-skeleton.css";
  import "@skeletonlabs/skeleton/styles/skeleton.css";
  import "../app.postcss";

  import Navbar from "$lib/components/navbar.svelte";
</script>


  <Navbar logo="Jorge Corzo" />
  <br />
  <slot />

