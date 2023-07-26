<script>
  import Icon from "@iconify/svelte";
  import { skills } from "$lib/config";
</script>

<!-- what i do section start -->
<div class="pb-12 px-6">
  <h3 class="h1 p-5 font-bold">What I do!</h3>
  <div class="grid gap-8 grid-cols-1 md:grid-cols-2">
    {#each skills as skill}
      <div
        class="border-2 rounded-xl dark:border-surface-800 border-surface-300 p-3"
      >
        <Icon icon={skill.icon} width="52" class="{skill.color}" />
        <div class="space-y-2">
          <h3 class=" text-[22px] font-semibold">{skill.name}</h3>
          <p class="leading-8">
            {skill.info}
          </p>
        </div>
      </div>
    {/each}
  </div>
</div>

<!-- what i do section finish -->
