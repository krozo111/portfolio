<script>
  import { educations, knowledges, workingSkills } from "$lib/config";
  import { experiences } from "$lib/config";
  import Icon from "@iconify/svelte";
</script>

<section class="container sm:px-5 md:px-10 lg:px-14 lg:rounded-2xl">
  <div class="py-12 px-4 md:px-0">
    <!-- resume page title -->
    <div class="flex h-12 items-center gap-3">
      <h2 class="h1 font-bold">Resume</h2>
      <div class=" h-0.5 w-40 bg-gradient-to-r from-orange-500 to-pink-500" />
    </div>
    <div
      class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-x-6 gap-y-6 mt-[30px]"
    >
      <!-- eductation start -->
      <div>
        <div class="flex items-center space-x-2 mb-4">
          <Icon icon="carbon:education" width="42" class="text-primary-500" />
          <h4 class="h2 font-medium">Education</h4>
        </div>
        {#each educations as education}
          <div
            class="bg-surface-50 dark:bg-transparent
              py-4 pl-5 pr-3 space-y-2 mb-6 rounded-lg
              dark:border-surface-700 dark:border-2"
          >
            <span class="text-tiny text-gray-lite dark:text-surface-400"
              >{education.year}</span
            >
            <h3 class="text-xl dark:text-white">{education.name}</h3>
            <p class="dark:text-[#b7b7b7]">{education.place}</p>
          </div>
        {/each}
      </div>
      <!-- eductation end -->

      <!-- experience start -->
      <div>
        <div class="flex items-center space-x-2 mb-4">
          <Icon
            icon="material-symbols:work-outline"
            width="42"
            class="text-primary-500"
          />
          <h4 class="h2 font-medium">Experience</h4>
        </div>
        {#each experiences as experience}
          <div
            class="py-4 pl-5 pr-3 space-y-2 mb-6
              rounded-lg bg-surface-50 dark:bg-transparent
               dark:border-[#212425] dark:border-2"
          >
            <span class="text-tiny text-gray-lite dark:text-[#b7b7b7]"
              >{experience.year}</span
            >
            <h3 class="text-xl dark:text-white">{experience.name}</h3>
            <p class="dark:text-[#b7b7b7]">{experience.place}</p>
          </div>
        {/each}
      </div>
      <!-- experience start -->
    </div>
  </div>
</section>

<!-- working section start -->
<section class="container py-12 px-2 sm:px-5 md:px-10 lg:px-20">
  <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <div class="col-span-1">
      <h4 class="h2 font-medium mb-6">Working Skills</h4>

      {#each workingSkills as workingSkill}
        <div class="mb-5">
          <div class="flex justify-between mb-1">
            <span class=" font-semibold text-primary-400"
              >{workingSkill.name}</span
            >
            <span class=" font-semibold text-[#526377] dark:text-[#A6A6A6"
              >{workingSkill.level}</span
            >
          </div>

          <div class="w-full bg-[#edf2f2] rounded-full h-1 dark:bg-[#1c1c1c]">
            <div
              class="{workingSkill.color} h-1 rounded-full"
              style="width: {workingSkill.level}"
            />
          </div>
        </div>
      {/each}
    </div>

    <div class="col-span-1">
      <h4 class="h2 font-medium mb-8">Knowledge</h4>
      <div class="flex gap-y-5 gap-x-2.5 flex-wrap">
        {#each knowledges as knowledge}
          <button class="resume-btn">{knowledge}</button>
        {/each}
      </div>
    </div>
  </div>
</section>
