<script>
  import profileImage from "$lib/images/hero_img.webp";
  import PersonalInfo from "../components/personalInfo.svelte";
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
    <div class="pt-[100px] pb-8">
      <h2 class="mt-6 mb-1 text-[26px] font-bold">Jorge Corzo large</h2>
      <h3
        class="mb-4 bg-surface-900 font-semibold inline-block px-5 py-1.5 rounded-lg"
      >
        FrontEnd Developer
      </h3>
      <div class="flex justify-center space-x-3">
        <!-- facebook icon and link -->
        <a
          href="https://www.facebook.com/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span class=""> ICONS </span>
        </a>
      </div>
      <PersonalInfo />
      <!-- download button -->
      <button class="button-base-styles bg-primary-500 rounded-3xl">
        <img class="h-5" src="./devstudio.png" alt="icon" />Download CV
      </button>
    </div>
  </div>
</div>
