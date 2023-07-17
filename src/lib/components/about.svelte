<script>
  import profileImage from "$lib/images/hero_img.webp"
</script>

<div
  class="container grid grid-cols-12 md:gap-10 justify-between lg:mt-[220px]"
>
  <!-- sidber personal info -->
  <div class="col-span-12 lg:col-span-4 hidden lg:block h-screen sticky top-44">
    <div
      class="w-full bg-surface-700 mb-6 lg:mb-0 mx-auto relative text-center px-6 rounded-[20px] mt-[180px] md:mt-[220px] lg:mt-0"
    >
      <!-- profile image -->
      <img
        src={profileImage}
        class="w-[240px] absolute left-[50%] transform -translate-x-[50%] h-[240px] drop-shadow-xl mx-auto rounded-[20px] -mt-[140px]"
        alt="about"
      />
      <div class="pt-[100px] pb-8">
        <h2 class="mt-6 mb-1 text-[26px] font-bold">Jorge Corzo about</h2>
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
  <div class="col-span-12 lg:col-span-8">
    <!-- header for mobile devices start -->
    <header
      class="bg-surface-700 lg:w-[560px] h-[144px] hidden lg:block p-[30px] ml-auto mb-10 rounded-[16px]"
    >
      <nav class="hidden lg:block">
        <ul class="flex justify-between text-tertiary-50 font-bold">
          <li>
            <a class="flex cursor-pointer flex-col items-center justify-center rounded-lg w-20 h-20 bg-gradient-to-r from-orange-500 to-pink-500" href="/">
              <span class="text-xl mb-1">
                <iconify-icon icon="mdi:about"></iconify-icon>
               
              </span> About
            </a>
          </li>
          <li>
            <a class="flex cursor-pointer flex-col items-center justify-center rounded-lg w-20 h-20 bg-gradient-to-r from-purple-500 to-pink-500" href="/">
              <span class="text-xl mb-1">
                <iconify-icon icon="mdi:resume"></iconify-icon>
              </span> Resume
            </a>
          </li>
          <li>
            <a class="flex cursor-pointer flex-col items-center justify-center rounded-lg w-20 h-20 bg-gradient-to-r from-purple-500 to-pink-500" href="/">
              <span class="text-xl mb-1">
                <iconify-icon icon="mdi:work"></iconify-icon>
              </span> Works
            </a>
          </li>
          <li>
            <a class="flex cursor-pointer flex-col items-center justify-center rounded-lg w-20 h-20 bg-gradient-to-r from-purple-500 to-pink-500" href="/">
              <span class="text-xl mb-1">
                <iconify-icon icon="mdi:blog"></iconify-icon>
              </span> Blogs
            </a>
          </li>
          <li>
            <a class="flex cursor-pointer flex-col items-center justify-center rounded-lg w-20 h-20 bg-gradient-to-r from-purple-500 to-pink-500" href="/">
              <span class="text-xl mb-1">
                <iconify-icon icon="mdi:contact"></iconify-icon>
              </span> Contact
            </a>
          </li>
        </ul>
      </nav>
    </header>
    <!-- header for mobile devices end -->

    <!-- about me section start -->
    <div>
      <div class="bg-surface-700 lg:rounded-2xl">
        <div class="pt-12 md:py-12 px-2 sm:px-5 md:px-10 lg:px-14">
          <!-- about page title -->
          <h2 class="after-effect after:left-52">About Me ?</h2>
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
                  Jorge Corzo Mobile
                </h2>
                <h3
                  class="mb-4 inline-block px-5 py-1.5 rounded-lg "
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
                    <span class="">
                     facebooks
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
                <div
                  class="p-7 rounded-2xl mt-7 bg-[#F3F6F6] dark:bg-[#1D1D1D]"
                >
                  <div
                    class="flex border-b border-[#E3E3E3] dark:border-[#3D3A3A] pb-2.5"
                  >
                    <span
                      class="socialbtn bg-white dark:bg-black text-[#E93B81] shadow-md"
                    >
                      <i class="fa-solid fa-mobile-screen-button" />
                    </span>
                    <div class="text-left ml-2.5">
                      <p class="text-xs text-[#44566C] dark:text-[#A6A6A6]">
                        Phone
                      </p>
                      <p class="dark:text-white">+123 456 7890</p>
                    </div>
                  </div>

                  <div
                    class="flex border-b border-[#E3E3E3] dark:border-[#3D3A3A] py-2.5"
                  >
                    <span
                      class="socialbtn bg-white dark:bg-black text-[#6AB5B9] shadow-md"
                    >
                      <i class="fa-solid fa-envelope-open-text" />
                    </span>
                    <div class="text-left ml-2.5">
                      <p class="text-xs text-[#44566C] dark:text-[#A6A6A6]">
                        Email
                      </p>
                      <p class="dark:text-white">example@mail.com</p>
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
                      <p class="dark:text-white">Hong kong china</p>
                    </div>
                  </div>

                  <div class="flex py-2.5">
                    <span
                      class="socialbtn bg-white dark:bg-black text-[#C17CEB] shadow-md"
                    >
                      <i class="fa-solid fa-calendar-days" />
                    </span>
                    <div class="text-left ml-2.5">
                      <p class="text-xs text-[#44566C] dark:text-[#A6A6A6]">
                        Birthday
                      </p>
                      <p class="dark:text-white">May 27, 1990</p>
                    </div>
                  </div>
                </div>
                <!-- personal info end -->

                <!-- dowanload button -->
                <button class="dowanload-btn">
                  <img
                    class="mr-3"
                    src={profileImage}
                    alt="icon"
                  /> Download CV
                </button>
              </div>
            </div>
          </div>
          <!-- personal info for mobile devices end -->

          <div
            class="lg:grid grid-cols-12 md:gap-10 pt-4 md:pt-[30px] items-center hidden"
          >
            <div class="col-span-12 space-y-2.5">
              <div class="lg:mr-16">
                <p class="text-[#44566c] dark:text-color-910 leading-7">
                  I'm Creative Director and UI/UX Designer from Sydney,
                  Australia, working in web development and print media. I enjoy
                  turning complex problems into simple, beautiful and intuitive
                  designs.
                </p>
                <p class="text-[#44566c] leading-7 mt-2.5 dark:text-color-910">
                  My aim is to bring across your message and identity in the
                  most creative way. I created web design for many famous brand
                  companies.
                </p>
              </div>
              <div />
            </div>
          </div>
        </div>

        <!-- what i do section start -->
        <div class="pb-12 px-2 sm:px-5 md:px-10 lg:px-14">
          <h3
            class="text-[35px] dark:text-white font-bold font-robotoSlab pb-5"
          >
            What I do!
          </h3>
          <div class="grid gap-8 grid-cols-1 md:grid-cols-2 xl:grid-cols-2">
            <div class="about-box bg-[#fcf4ff] dark:bg-transparent">
              <img
              class="w-10 h-10 object-contain block"
              src={profileImage}
              alt="icon"
            />
              <div class="space-y-2">
                <h3 class=" text-[22px] font-semibold">
                  Ui/Ux Design
                </h3>
                <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed
                  diam euismod volutpat.
                </p>
              </div>
            </div>

            <div class="about-box bg-[#fefaf0] dark:bg-transparent">
              <img
                class="w-10 h-10 object-contain block"
                src={profileImage}
                alt="icon"
              />
              <div class="space-y-2">
                <h3 class="dark:text-white text-[22px] font-semibold">
                  App Development
                </h3>
                <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed
                  diam euismod volutpat.
                </p>
              </div>
            </div>

            <div class="about-box bg-[#fcf4ff] dark:bg-transparent">
              <img
                class="w-10 h-10 object-contain block"
                src={profileImage}
                alt="icon"
              />
              <div class="space-y-2">
                <h3 class="dark:text-white text-[22px] font-semibold">
                  Photography
                </h3>
                <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed
                  diam euismod volutpat.
                </p>
              </div>
            </div>

            <div class="about-box bg-[#fff4f4] dark:bg-transparent">
              <img
                class="w-10 h-10 object-contain block"
                src={profileImage}
                alt="icon"
              />
              <div class="space-y-2">
                <h3 class="dark:text-white text-[22px] font-semibold">
                  Photography
                </h3>
                <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed
                  diam euismod volutpat.
                </p>
              </div>
            </div>

            <div class="about-box bg-[#fff0f8] dark:bg-transparent">
              <img
                class="w-10 h-10 object-contain block"
                src={profileImage}
                alt="icon"
              />
              <div class="space-y-2">
                <h3 class="dark:text-white text-[22px] font-semibold">
                  Managment
                </h3>
                <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed
                  diam euismod volutpat.
                </p>
              </div>
            </div>

            <div class="about-box bg-[#f3faff] dark:bg-transparent">
              <img
                class="w-10 h-10 object-contain block"
                src={profileImage}
                alt="icon"
              />
              <div class="space-y-2">
                <h3 class="dark:text-white text-[22px] font-semibold">
                  Web Development
                </h3>
                <p class="leading-8 text-gray-lite dark:text-[#A6A6A6]">
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed
                  diam euismod volutpat.
                </p>
              </div>
            </div>
          </div>
        </div>

        <!-- what i do section start -->
        <div class="px-2 sm:px-5 md:px-10 lg:px-14">
          <div
            class="bg-[#F8FBFB] dark:bg-[#0D0D0D] max-w-full h-auto py-10 rounded-xl"
          >
            <h3 class="text-center dark:text-white text-6xl mb-3 font-semibold">
              Clients
            </h3>
            <!-- slider and slider items -->
            <div
              class="slickOne text-center px-2 pt-8 slick-initialized slick-slider"
            >
              <div class="slick-list draggable">
                <div
                  class="slick-track"
                  style="opacity: 1; width: 2340px; transform: translate3d(-910px, 0px, 0px); transition: transform 500ms ease 0s;"
                >
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="-4"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="-3"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="-2"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="-1"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="0"
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="1"
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  
                  <div
                    class="slick-slide slick-active"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="6"
                    aria-hidden="false"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="7"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="8"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="9"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="10"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="11"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="12"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                  <div
                    class="slick-slide slick-cloned"
                    style="width: 130px;"
                    tabindex="-1"
                    data-slick-index="13"
                    id=""
                    aria-hidden="true"
                  >
                    <img
                      class="overflow-hidden brand-img"
                      src={profileImage}
                      alt="brand icon"
                    />
                  </div>
                </div>
              </div>
            </div>
            <!-- slider and slider items end -->
          </div>
        </div>

        <!-- footer start -->
        <footer
          class="overflow-hidden rounded-b-2xl"
          style="background: transparent"
        >
          <p class="text-center py-6 text-gray-lite dark:text-color-910">
            © 2022 All Rights Reserved by <a
              class="hover:text-[#FA5252] duration-300 transition"
              href="https://themeforest.net/user/ib-themes"
              target="_blank"
              rel="noopener noreferrer"
            >
              ib-themes</a
            >.
          </p>
        </footer>
        <!-- footer section end -->
      </div>
    </div>
    <!-- about me section start -->
  </div>
</div>
