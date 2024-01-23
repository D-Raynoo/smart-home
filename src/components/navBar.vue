<template>
  <nav
    class="flex pt-[3vw] px-8 lg:pt-12 justify-around items-center text-lg font-bold"
  >
    <!-- -----------------------------logo--------------------------- -->
    <div class="z-50 w-[20%] lg:w-40 h-auto">
      <img
        src="../assets/Landing-page/Logo/Logo.png"
        alt=""
        class="w-full h-auto m-0 lg:px-10"
      />
    </div>
    <!-- ---------------------------menu-------------------------------- -->
    <div
      class="lg:flex justify-between items-center z-40 lg:w-[30rem] lg:h-auto lg:mr-16 lg:shadow-none overflow-hidden lg:overflow-visible h-96 lg:p-0 lg:rounded-none font-medium rounded-lg w-full absolute top-0 pt-28 lg:static lg:backdrop-blur-none"
      :class="open ? 'backdrop-blur-md shadow-md animate-fade-down' : ' hidden'"
    >
      <a
        v-for="(link, index) in links"
        :key="index"
        link
        :to="link.link"
        href=""
        :class="open ? '' : 'opacity-0 translate-x-96 blur-md'"
        class="group block mt-5 w-full lg:text-lg lg:w-auto text-center lg:text-left lg:translate-x-0 lg:opacity-100 lg:blur-none lg:inline-block lg:mt-0 max-w-full whitespace-nowrap text-white"
      >
        {{ link.name
        }}<span
          class="block text-top max-w-0 group-hover:max-w-full transition-all duration-500 h-0.5 bg-white"
        ></span
      ></a>
    </div>
    <!-- -----------------------------search bar-------------------------------- -->
    <div
      class="relative z-50 text-white flex w-full items-center mx-8 lg:mx-0 overflow-hidden rounded-full lg:w-64 lg:h-9 lg:mr-8"
    >
      <input
        type="search"
        name="search"
        class="bg-transparent indent-3 border border-solid overflow-hidden border-white h-[6vw] lg:h-full w-full rounded-full text-sm focus:outline-none"
        @focusin="translateLabelPosition = true"
        @focusout="translateLabelPosition = false"
      />
      <label
        for="search"
        class="absolute font-medium pointer-events-none select-none right-6 items-center text-[3vw] lg:text-lg fill-current block transition-all duration-1000 ease"
        :class="translateLabelPosition ? 'translate-x-56' : ''"
      >
        Search
      </label>
      <svg
        style="color: white"
        xmlns="http://www.w3.org/2000/svg"
        width="20"
        height="20"
        fill="currentColor"
        class="bi bi-search cursor-pointer right-5 absolute items-center text-base block transition-all duration-1000 ease hover:animate-shake"
        :class="!translateLabelPosition ? 'translate-x-56' : ''"
        viewBox="0 0 16 16"
      >
        <path
          d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"
          fill="white"
        ></path>
      </svg>
    </div>
    <!-- -----------------------social media icons------------------------ -->
    <div
      class="flex z-50 items-center space-x-[8%] justify-around transition-all ease-in duration-500 w-full lg:w-36 lg:opacity-100 absolute top-[21rem] lg:static"
    >
      <a
        class="hover:scale-75 lg:blur-none lg:block lg:w-1/4 lg:opacity-100 lg:translate-x-0 transition-all ease-in"
        :class="open ? 'animate-fade-down' : 'hidden'"
        href=""
        ><img
          src="../assets/Landing-page/Social Media Icons/Instagram.png"
          alt=""
          class="block w-full h-auto"
      /></a>
      <a
        class="hover:scale-75 lg:blur-none lg:block lg:w-1/4 lg:opacity-100 lg:translate-x-0 transition-all ease-in duration-100"
        :class="open ? 'animate-fade-down' : 'hidden'"
        href=""
        ><img
          src="../assets/Landing-page/Social Media Icons/Facebook.png"
          alt=""
          class="block w-full h-auto"
      /></a>
      <a
        class="hover:scale-75 lg:blur-none lg:block lg:w-1/4 lg:opacity-100 lg:translate-x-0 transition-all ease-in duration-200"
        :class="open ? 'animate-fade-down' : 'hidden'"
        href=""
        ><img
          src="../assets/Landing-page/Social Media Icons/Twitter.png"
          alt=""
          class="block w-full h-auto"
      /></a>
      <a
        class="hover:scale-75 lg:blur-none lg:block lg:w-1/4 lg:opacity-100 lg:translate-x-0 transition-all ease-in duration-300"
        :class="open ? 'animate-fade-down' : 'hidden'"
        href=""
        ><img
          src="../assets/Landing-page/Social Media Icons/WhatsApp.png"
          alt=""
          class="block w-full h-auto"
      /></a>
    </div>
    <!-- ------------------------menu button for sm&md-------------------------- -->
    <button
      class="text-white z-50 w-12 h-12 relative focus:outline-none bg-transparent lg:hidden"
      @click="open = !open"
    >
      <span class="sr-only">Open main menu</span>
      <div
        class="block w-full absolute left-1/2 top-1/2 transform -translate-x-1/2 -translate-y-1/2"
      >
        <span
          aria-hidden="true"
          class="block absolute h-1 w-full bg-current transform transition duration-500 ease-in-out"
          :class="{ 'rotate-45': open, ' -translate-y-1.5': !open }"
        ></span>
        <span
          aria-hidden="true"
          class="block absolute h-1 w-full bg-current transform transition duration-500 ease-in-out"
          :class="{ 'opacity-0': open }"
        ></span>
        <span
          aria-hidden="true"
          class="block absolute h-1 w-full bg-current transform transition duration-500 ease-in-out"
          :class="{ '-rotate-45': open, ' translate-y-1.5': !open }"
        ></span>
      </div>
    </button>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      translateLabelPosition: false,
      open: false,
      links: [
        {
          name: "Home",
          path: "#",
          transitionDuration: "",
        },
        {
          name: "About",
          path: "#",
          transitionDuration: "duration-100",
        },
        {
          name: "Access Control",
          path: "#",
          transitionDuration: "duration-200",
        },
        {
          name: "Digital",
          path: "#",
          transitionDuration: "duration-300",
        },
      ],
      socialMediaLinks: [
        {
          name: "Instagram",
          path: "#",
          icon: "../assets/Landing-page/Social Media Icons/Instagram.png",
        },
        {
          name: "Facebook",
          path: "#",
          icon: "../assets/Landing-page/Social Media Icons/Facebook.png",
        },
        {
          name: "Twitter",
          path: "#",
          icon: "../assets/Landing-page/Social Media Icons/Twitter.png",
        },
        {
          name: "WhatsApp",
          path: "#",
          icon: "../assets/Landing-page/Social Media Icons/WhatsApp.png",
        },
      ],
    };
  },
};
</script>

<style>
</style>