<script>
  import "@skeletonlabs/skeleton/themes/theme-crimson.css";
  import "@skeletonlabs/skeleton/styles/skeleton.css";
  import "../app.postcss";
  import "iconify-icon";
  import Navbar from "$lib/components/navbar.svelte";
  import SideNav from "$lib/components/sideNav.svelte";
  import Footer from "$lib/components/footer.svelte";
  import Navbar2 from "$lib/components/navbar2.svelte";
  import profileImage from "$lib/images/hero_img.webp";
  import PersonalInfo from "$lib/components/personalInfo.svelte";
</script>

<svelte:head>
  <title>Jorge Corzo - Portfolio</title>
</svelte:head>

<div class="hidden lg:block px-6">
  <div class="container grid grid-cols-12 gap-10 justify-between mt-[220px]">
    <SideNav />
    <div class="col-span-12 lg:col-span-8">
      <Navbar />
      <div class="bg-surface-700 rounded-2xl">
        <slot />
        <Footer />
      </div>
    </div>
  </div>
</div>

<div class="lg:hidden">
  <div class="col-span-12">
    <!-- header for mobile devices start -->
    <Navbar2 />
    <!-- about me section start -->
    <div class="pt-12 md:py-12 px-2 sm:px-5 md:px-10 lg:px-14">
      <!-- personal info for mobile devices start -->
      <div class="lg:hidden">
        <div
          class="w-full mb-6 lg:mb-0 mx-auto relative text-center px-6 rounded-[20px] mt-[180px] md:mt-[220px] lg:mt-0"
        >
          <!-- profile image  -->
          <img
            src={profileImage}
            class="w-[240px] absolute left-[50%] transform -translate-x-[50%] h-[240px] drop-shadow-xl mx-auto rounded-[20px] -mt-[140px]"
            alt="about"
          />
          <div class="pt-[100px] pb-8">
            <h2 class="mt-6 mb-1 text-[26px] font-semibold">
              Jorge Corzo Sample
            </h2>
            <h3 class="mb-4inline-block px-5 py-1.5 rounded-lg">
              FrontEnd Developer
            </h3>

            <div class="flex justify-center space-x-3">
              <!-- facebook icon and link -->
              <a
                href="https://www.facebook.com/jorge.corzo"
                target="_blank"
                rel="noopener noreferrer"
              >
                <span class="socialbtn text-[#1773EA]">
                  <i class="fa-brands fa-facebook-f" />F
                </span>
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
      <!-- personal info for mobile devices end -->
      <slot />
      <Footer />
    </div>
  </div>
</div>
