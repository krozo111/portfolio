<script>
  import Icon from '@iconify/svelte';
  import { personalInfo } from '$lib/config';
  import profileImage from "$lib/images/hero_img.webp";
  import PersonalInfo from "../components/personalInfo.svelte";
  import Button from './button.svelte';
</script>

<!-- sidber personal info -->
<div class=" col-span-12 lg:col-span-4 h-screen sticky">
  <div
    class="w-full bg-surface-700 mb-6 mx-auto text-center px-6 rounded-[20px] mt-[180px] lg:mt-0"
  >
    <!-- profile image -->
    <img
      src={profileImage}
      class="w-[240px] absolute left-[50%] transform -translate-x-[50%] h-[240px] drop-shadow-xl mx-auto rounded-[20px] -mt-[140px]"
      alt="about"
    />
    <div class="pt-[100px] pb-4">
      <h2 class="mt-6 mb-4 h2 font-bold">{personalInfo.name}</h2>
      <h5
        class="mb-4 h5 bg-surface-900 inline-block px-5 py-1.5 rounded-lg"
      >
       {personalInfo.ocupation}
      </h5>
      <div class="flex justify-center space-x-3">
        <!-- facebook icon and link -->
        <a
          href="https://www.facebook.com/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span class="">
            <Icon icon="openmoji:facebook" width="36" height="36" />
          </span>
        </a>
        <a
        href="https://www.github.com/krozo111"
        target="_blank"
        rel="noopener noreferrer"
      >
        <span class="">
          <Icon icon="openmoji:github" width="36" height="36" />
        </span>
      </a>
      <a
      href="https://www.instagram.com/jorgecorzoh"
      target="_blank"
      rel="noopener noreferrer"
    >
      <span class="">
        <Icon icon="openmoji:instagram" width="36" height="36" />
      </span>
    </a>
      </div>
      <PersonalInfo />
      <!-- download button -->
      <Button />
    </div>
  </div>
</div>
