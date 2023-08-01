<script>
  import { works } from "$lib/config";
</script>

<div class="container px-4 sm:px-5 md:px-10 lg:px-[60px]">
  <div class="py-12 px-4 md:px-0">
    <div class="flex h-12 items-center gap-3 mb-10">
      <h2 class="h1 font-bold">Portfolio</h2>
      <div class=" h-0.5 w-40 bg-gradient-to-r from-orange-500 to-pink-500" />
    </div>
    <main class="grid grid-cols-2 gap-10">
      {#each works as work}
        <card class="card card-hover overflow-hidden">
          <header>
            <img
              src="https://images.unsplash.com/photo-1620562303747-ba21ca6f1530?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY2MjR8&amp;ixlib=rb-4.0.3&amp;w=400&amp;h=175&amp;auto=format&amp;fit=crop"
              class="w-full aspect-[21/9]"
              alt={work.name}
            />
          </header>
          <div class="p-4 space-y-4">
            <h6 class="h6">{work.name}</h6>
            <h3 class="h3" data-toc-ignore="">{work.technology}</h3>
            <article>
              <p>{work.description}.</p>
            </article>
          </div>
          <hr class="opacity-50" />
          
        </card>
      {/each}
    </main>
  </div>
</div>
