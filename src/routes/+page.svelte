<script>
  import Main from "$lib/components/main.svelte";
  import Sample from "$lib/components/sample.svelte";
</script>

<svelte:head>
  <title>Jorge Corzo - Portfolio</title>
</svelte:head>

<main class="hidden lg:block px-6">
  <Main />
</main>

<div class="lg:hidden">
  <Sample />
</div>

<style>
</style>
