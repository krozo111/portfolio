<script>
  import Footer from "./footer.svelte";
  import Navbar from "./navbar.svelte";
  import profileImage from "$lib/images/hero_img.webp";
</script>

<div class="col-span-12">
  <!-- header for mobile devices start -->
  <header class="relative h-[144px] p-[30px] ml-auto mb-10 rounded-[16px]">
    <p class="fixed top-0">Header</p>
  </header>
  <!-- header for mobile devices end -->

  <!-- about me section start -->

  <div class="">
    <div class="pt-12 md:py-12 px-2 sm:px-5 md:px-10 lg:px-14">
      <!-- about page title -->
      <h2 class="h1">About Me</h2>
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
                href="https://www.facebook.com/"
                target="_blank"
                rel="noopener noreferrer"
              >
                <span class="socialbtn text-[#1773EA]">
                  <i class="fa-brands fa-facebook-f" />
                </span>
              </a>
              <!-- twitter icon and link -->
              <a
                href="https://twitter.com/"
                target="_blank"
                rel="noopener noreferrer"
              >
                <span class="socialbtn text-[#1C9CEA]">
                  <i class="fa-brands fa-twitter" />
                </span>
              </a>
              <!-- dribbble icon and link -->
              <a
                href="https://dribbble.com/"
                target="_blank"
                rel="noopener noreferrer"
              >
                <span class="socialbtn text-[#e14a84]">
                  <i class="fa-brands fa-dribbble" />
                </span>
              </a>
              <!-- linkedin icon and link -->
              <a
                href="https://www.linkedin.com/"
                target="_blank"
                rel="noopener noreferrer"
              >
                <span class="socialbtn text-[#0072b1]">
                  <i class="fa-brands fa-linkedin-in" />
                </span>
              </a>
            </div>

            <!-- personal info start -->
            <div class="p-7 rounded-2xl mt-7 bg-[#F3F6F6] dark:bg-[#1D1D1D]">
              <div
                class="flex border-b border-[#E3E3E3] dark:border-[#3D3A3A] pb-2.5"
              >
                <span
                  class="socialbtn bg-white dark:bg-black text-[#E93B81] shadow-md"
                >
                  <i class="fa-solid fa-mobile-screen-button" />
                </span>
                <div class="text-left ml-2.5">
                  <p class="text-xs">Phone</p>
                  <p class="">+123 456 7890</p>
                </div>
              </div>

              <div class="flex border-b border-[#E3E3E3] py-2.5">
                <span class="socialbtn shadow-md">
                  <i class="fa-solid fa-envelope-open-text" />
                </span>
                <div class="text-left ml-2.5">
                  <p class="text-xs">Email</p>
                  <p class=" ">example@mail.com</p>
                </div>
              </div>

              <div
                class="flex border-b border-[#E3E3E3] dark:border-[#3D3A3A] py-2.5"
              >
                <span
                  class="socialbtn bg-white dark:bg-black text-[#FD7590] shadow-md"
                >
                  <i class="fa-solid fa-location-dot" />
                </span>
                <div class="text-left ml-2.5">
                  <p class="text-xs text-[#44566C] dark:text-[#A6A6A6]">
                    Location
                  </p>
                  <p class=" ">Hong kong china</p>
                </div>
              </div>

              <div class="flex py-2.5">
                <span class="socialbtnshadow-md">
                  <i class="fa-solid fa-calendar-days" />
                </span>
                <div class="text-left ml-2.5">
                  <p class="text-xs">Birthday</p>
                  <p class=" ">May 27, 1990</p>
                </div>
              </div>
            </div>
            <!-- personal info end -->

            <!-- dowanload button -->
            <button class="button-base-styles bg-primary-500 rounded-3xl">
              <img class="h-5" src="./devstudio.png" alt="icon" />Download CV
            </button>
          </div>
        </div>
      </div>
      <!-- personal info for mobile devices end -->

      <div
        class="lg:grid grid-cols-12 md:gap-10 pt-4 md:pt-[30px] items-center"
      >
        <div class="col-span-12 space-y-2.5">
          <div class="lg:mr-16">
            <p class="leading-7">
              I'm Creative Director and UI/UX Designer from Sydney, Australia,
              working in web development and print media. I enjoy turning
              complex problems into simple, beautiful and intuitive designs.
            </p>
            <p class=" leading-7 mt-2.5">
              My aim is to bring across your message and identity in the most
              creative way. I created web design for many famous brand
              companies.
            </p>
          </div>
          <div />
        </div>
      </div>
    </div>

    <!-- what i do section start -->
    <div class="pb-12 px-2 sm:px-5 md:px-10 lg:px-14">
      <h3 class="text-[35px] font-bold font-robotoSlab pb-5">What I do!</h3>
      <div class="grid gap-8 grid-cols-1 md:grid-cols-2 xl:grid-cols-2">
        <div class="about-box">
          <img
            class="w-10 h-10 object-contain block"
            src={profileImage}
            alt="icon"
          />
          <div class="space-y-2">
            <h3 class="  text-[22px] font-semibold">Ui/Ux Design</h3>
            <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam
              euismod volutpat.
            </p>
          </div>
        </div>

        <div class="about-box">
          <img
            class="w-10 h-10 object-contain block"
            src={profileImage}
            alt="icon"
          />
          <div class="space-y-2">
            <h3 class="  text-[22px] font-semibold">App Development</h3>
            <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam
              euismod volutpat.
            </p>
          </div>
        </div>

        <div class="about-box">
          <img
            class="w-10 h-10 object-contain block"
            src={profileImage}
            alt="icon"
          />
          <div class="space-y-2">
            <h3 class="  text-[22px] font-semibold">Photography</h3>
            <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam
              euismod volutpat.
            </p>
          </div>
        </div>

        <div class="about-box">
          <img
            class="w-10 h-10 object-contain block"
            src={profileImage}
            alt="icon"
          />
          <div class="space-y-2">
            <h3 class="  text-[22px] font-semibold">Photography</h3>
            <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam
              euismod volutpat.
            </p>
          </div>
        </div>

        <div class="about-box">
          <img
            class="w-10 h-10 object-contain block"
            src={profileImage}
            alt="icon"
          />
          <div class="space-y-2">
            <h3 class="  text-[22px] font-semibold">Managment</h3>
            <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam
              euismod volutpat.
            </p>
          </div>
        </div>

        <div class="about-box">
          <img
            class="w-10 h-10 object-contain block"
            src={profileImage}
            alt="icon"
          />
          <div class="space-y-2">
            <h3 class="  text-[22px] font-semibold">Web Development</h3>
            <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam
              euismod volutpat.
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- what i do section start -->
    <div class="px-2 sm:px-5 md:px-10 lg:px-14">
      <div class="max-w-full h-auto py-10 rounded-xl">
        <h3 class="text-center text-6xl mb-3 font-semibold">Clients</h3>
        <!-- slider and slider items -->
        <p class="text-center">Slider here</p>
        <!-- slider and slider items end -->
      </div>
    </div>

    <!-- footer start -->
    <Footer />
    <!-- footer section end -->
  </div>
</div>
<!-- about me section start -->
