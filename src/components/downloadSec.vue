<template>
  <section
    class="lg:flex justify-center gap-10 items-center py-20 px-14 text-white"
  >
    <div
      class="lg:flex-column justify-center mb-6 lg:mb-52 items-center mx-auto w-full lg:w-fit"
    >
      <div class="lg:w-fit w-full lg:mx-auto">
        <h2
          class="font-['Audiowide'] text-[2.5rem] text-center leading-none lg:text-left lg:w-min"
        >
          MONITOR HOME REMOTELY
        </h2>

        <ul
          class="text-xl sm:text-4xl lg:text-[1.45rem] px-4 lg:px-0 mt-6 lg:mt-28 text-[4vw] lg:w-fit lg:whitespace-nowrap tracking-wide lg:text-left"
        >
          <li
            class="mb-2 leading-tight before:content-['·'] before:content-center before:text-[6vw] before:md:text-[2.5vw]"
          >
            Lorem ipsum dolor sit amet, consectetur<br />adipiscing elit, sed do
            eiusmod tempor
          </li>

          <li
            class="mb-2 leading-tight before:content-['·'] before:content-center before:text-[6vw] before:md:text-[2.5vw]"
          >
            incididunt ut labore et dolore magna aliqua.
          </li>

          <li
            class="mb-2 leading-tight before:content-['·'] before:content-center before:text-[6vw] before:md:text-[2.5vw]"
          >
            Ut enim ad minim veniam, quis nostrud<br />exercitation ullamco
            laboris nisi ut aliquip ex<br />ea<br />commodo consequat. Duis aute
            irure dolor in
          </li>

          <li
            class="mb-2 leading-tight before:content-['·'] before:content-center before:text-[6vw] before:md:text-[2.5vw]"
          >
            reprehenderit in voluptate velit esse cillum<br />dolore eu fugiat
            nulla pariatur. Excepteur sint<br />occaecat cupidatat non proident,
            sunt in
          </li>
        </ul>
      </div>

      <div class="my-6 lg:my-14">
        <h3 class="md:text-4xl text-[8vw] font-bold italic tracking-widexx">
          Service
        </h3>
        <h1
          class="md:text-6xl text-[14vw] font-bold italic tracking-[1rem] leading-none"
        >
          012345
        </h1>
      </div>

      <div class="flex-column items-center">
        <h3 class="tracking-widex font-medium text-[3.25vw] mb-4 md:text-2xl">
          DOWNLOAD AVAIBLE ON
        </h3>
        <button
          class="border-solid border-2 border-white w-[30vw] md:w-48 mr-4 h-12 md:h-16 hover:shadow-fuchsia-700 hover:scale-110 transition-all ease-in duration-200 shadow-lg"
        ></button
        ><button
          class="border-solid border-2 border-white w-[30vw] md:w-48 ml-4 h-12 md:h-16 hover:shadow-fuchsia-700 hover:scale-110 transition-all ease-in duration-200 shadow-lg"
        ></button>
      </div>
    </div>
    <intersect @enter="isObservable = true" @leave="isObservable = false">
      <div
        class="grid place-items-center lg:my-6 w-full lg:w-1/2 h-auto"
        :class="isObservable ? ' animate-fade-left' : ''"
      >
        <img
          src="../assets/Landing-page/Smartphone.png"
          alt=""
          class="h-auto w-2/3 lg:w-full mx-auto max-w-xl"
        />
      </div>
    </intersect>
  </section>
</template>

<script>
import intersect from "vue-intersect";
export default {
  data() {
    return {
      isObservable: false,
    };
  },
  components: {
    intersect,
  },
};
</script>

<style>
</style>