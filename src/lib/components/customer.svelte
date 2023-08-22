<script>
  import {clients} from "../config";
</script>

<main class="justify-center align-middle px-6 pb-6 rounded-xl">
  <h1 class="flex h1 pt-5 font-bold">Clients</h1>
  <div class="snap-x scroll-px-4 snap-mandatory scroll-smooth flex gap-2 overflow-x-auto py-8">
    {#each clients as client }
      <div class="snap-center shrink-0 card py-14 w-60 text-center">
        <img src={client.src} alt={client.name}>
      </div>
    {/each}
  </div>
</main>
