<script>
  import Icon from "@iconify/svelte";
  import { personalInfo } from "$lib/config";
  import { socialLinks } from "$lib/config";
  import PersonalInfo from "../components/personalInfo.svelte";
  import Button from "./button.svelte";
  
</script>

<!-- sidber personal info -->

  <div
    class="lg:sticky lg:top-48 bg-surface-200 dark:bg-black mx-auto text-center px-10 rounded-[20px]"
  >
    <!-- profile image -->
    <img
      src={personalInfo.img}
      class=" w-[240px]  h-[240px] drop-shadow-xl mx-auto rounded-[20px] lg:-mt-[180px]"
      alt="about"
    />
    <div class="py-4">
      <h2 class="mt-6 mb-4 h2 font-bold">{personalInfo.name}</h2>
      <h5
        class="mb-4 h5 bg-surface-50 dark:bg-surface-900 inline-block px-5 py-1.5 rounded-lg"
      >
        {personalInfo.ocupation}
      </h5>
      <div class="flex justify-center space-x-3">
        <!-- facebook icon and link -->
        {#each socialLinks as socialLink}
          <li class="list-none">
            <a
              id={socialLink.name}
              href={socialLink.href}
              target="_blank"
              rel="noopener noreferrer"
            >
              <span class="">
                <Icon
                  icon={socialLink.icon}
                  width="36"
                  height="36"
                  color="black dark:white"
                />
              </span>
            </a>
          </li>
        {/each}
      </div>
      <PersonalInfo />
      <!-- download button -->
      <div id="boton"><Button >Download CV </Button > </div>
    </div>
  </div>

