<script>
  import About from "$lib/components/about.svelte";
  import { works } from "$lib/config";
</script>

<div class=" px-4 sm:px-5 md:px-10 lg:px-[60px]">
  <div class="py-12 px-4 md:px-0">
    <div class="flex h-12 items-center gap-3 mb-10">
      <h2 class="h1 font-bold">Portfolio</h2>
      <div class=" h-0.5 w-40 bg-gradient-to-r from-orange-500 to-pink-500" />
    </div>
    <main class="md:grid md:grid-cols-2 gap-10">
      {#each works as work}
        <card class="">
          <header>
            <img src={work.src} class="h-fit" alt={work.name} />
          </header>
          <div class="p-4">
            <a href={work.link} target="_blank" class="h3 hover:text-red-500">{work.name}</a>
            <p>{work.description}.</p> <br />
              <p class="">Made with.. {work.technology}</p>
          
          </div>
          <hr class="opacity-50" />
        </card>
      {/each}
    </main>
  </div>
</div>
