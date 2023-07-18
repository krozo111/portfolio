<script>
  import About from "./about.svelte";
  import profileImage from "$lib/images/hero_img.webp";
</script>

<div class="container grid grid-cols-12 gap-10 justify-between mt-[220px]">
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
        <!-- personal infomation start -->
        <div class="p-7 rounded-2xl mt-7 bg-surface-900">
          <div class="flex border-b pb-2.5">
            <span class="socialbtn shadow-md">
              <i class="">Icon</i>
            </span>
            <div class="text-left ml-2.5">
              <p class="text-xs">Phone</p>
              <p class="">+123 456 7890</p>
            </div>
          </div>
          <div class="flex border-b py-2.5">
            <span class="socialbtnshadow-md">
              <i class="" />
            </span>
            <div class="text-left ml-2.5">
              <p class="text-xs">Email</p>
              <p class="">example@mail.com</p>
            </div>
          </div>
          <div class="flex border-b py-2.5">
            <span class="">
              <i class="">I</i>
            </span>
            <div class="text-left ml-2.5">
              <p class="text-xs">Location</p>
              <p class="">Hong kong china</p>
            </div>
          </div>
          <div class="flex py-2.5">
            <span class="">
              <i class="" />
            </span>
            <div class="text-left ml-2.5">
              <p class="text-xs">Birthday</p>
              <p class="">May 27, 1986</p>
            </div>
          </div>
        </div>
        <!-- personal infomation end-->
        <!-- dowanload button -->
        <button class="button-base-styles bg-primary-500"> Download CV </button>
      </div>
    </div>
  </div>
  <About />
</div>
