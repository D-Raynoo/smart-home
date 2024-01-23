<template>
  <section
    class="lg:flex items-center py-20 px-4 lg:px-14 gap-10 justify-center"
  >
    <div
      class="hidden lg:flex items-center justify-center w-[45%] max-w-2xl h-auto"
    >
      <img
        src="../assets/Landing-page/Home Design 3/Vector Smart Object (Double Click to Edit).png"
        alt=""
        class="block w-full h-auto"
      />
    </div>
    <div class="text-white lg:w-fit lg:text-left h-auto">
      <h2
        class="font-['Audiowide'] text-[2.5rem] mb-6 lg:mb-0 lg:text-[5.5rem] lg:w-fit leading-none lg:whitespace-nowrap lg:pr-5"
      >
        SMART HOME
      </h2>

      <h3
        class="text-xl sm:text-4xl lg:text-[1.45rem] lg:whitespace-nowrap mb-10 lg:w-fit tracking-wide lg:mb-8 lg:mt-16"
      >
        Lorem ipsum dolor sit amet, consectetur adipiscing<br />elit, sed do
        eiusmod tempor incididunt ut labore et<br />dolore magna aliqua. Ut enim
        ad minim veniam, quis<br />nostrud exercitation ullamco laboris nisi ut
        aliquip ex<br />ea commodo consequat. Duis aute irure dolor in<br />reprehenderit
        in voluptate velit esse cillum dolore eu<br />fugiat nulla pariatur.
        Excepteur sint occaecat cupidatat<br />
        non proident, sunt in culpa qui officia deserunt molli<br />
        anim id est laborum.
      </h3>

      <button
        class="border-solid border border-white text-[4vw] ml-0 lg:float-left sm:text-4xl lg:text-2xl px-[5.5vw] py-[0.5vw] md:py-2 md:px-16 rounded-full hover:shadow-fuchsia-700 hover:scale-110 transition-all ease-in duration-200 shadow-lg"
      >
        Read More
      </button>
    </div>
    <div class="lg:hidden flex justify-center mt-8 items-center w-full h-auto">
      <img
        src="../assets/Landing-page/Home Design 3/Vector Smart Object (Double Click to Edit).png"
        alt=""
        class="block w-full h-auto"
      />
    </div>
  </section>
</template>

<script>
import intersect from "vue-intersect";
export default {
  data() {
    return {
      buttonIsObservable: false,
    };
  },
  components: {
    intersect,
  },
};
</script>

<style>
</style>