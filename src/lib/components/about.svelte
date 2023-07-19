<script>
  import Footer from "./footer.svelte";
  import Navbar from "./navbar.svelte";
  import Skills from "./skills.svelte";
</script>

<div class="col-span-12 lg:col-span-8">
  <!-- header for desktop devices start -->
  <Navbar />
  <!-- about me section start -->
  <div>
    <div class="bg-surface-700 rounded-2xl">
      <div class="pt-12 md:py-12 px-2 md:px-10 lg:px-14">
        <!-- about page title -->
        <h2 class="h1">About Me</h2>

        <div
          class="lg:grid grid-cols-12 md:gap-10 pt-4 md:pt-[30px] items-center hidden"
        >
          <div class="col-span-12 space-y-2.5">
            <div class="lg:mr-16">
              <p class="leading-7">
                I'm Creative Director and UI/UX Designer from Sydney, Australia,
                working in web development and print media. I enjoy turning
                complex problems into simple, beautiful and intuitive designs.
              </p>
              <p class="mt-2.5 leading-7">
                My aim is to bring across your message and identity in the most
                creative way. I created web design for many famous brand
                companies.
              </p>
            </div>
            <div />
          </div>
        </div>
      </div>

      <Skills />

      <!-- clients -->
      <div class="px-2 md:px-10 lg:px-14 h-screen">
        <div class="max-w-full h-auto py-10 rounded-xl">
          <h3 class="text-center text-6xl mb-3 font-semibold">Clients</h3>
        </div>
      </div>

      <Footer />
    </div>
  </div>
</div>
