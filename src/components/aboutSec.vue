<template>
  <section
    class="lg:grid grid-rows-[100%] grid-cols-[35%,65%] lg:grid-cols-[50%,50%] place-items-center py-20 lg:px-14"
  >
    <div
      class="hidden lg:flex items-center justify-end w-full h-auto"
      :class="isObservable ? 'animate-fade-left ' : ''"
    >
      <img
        src="../assets/Landing-page/Home Design 4/Vector Smart Object (Double Click to Edit).png"
        alt=""
        class="block w-[85%] max-w-3xl lg:pt-[6vw] h-auto"
      />
    </div>
    <intersect @enter="isObservable = true" @leave="isObservable = false">
      <div
        class="text-white lg:pl-[3vw] h-auto place-self-center justify-self-start"
        :class="isObservable ? 'animate-fade-left ' : ''"
      >
        <h2
          class="text-[2.5rem] leading-none lg:leading-normal tracking-widex lg:text-left font-bold"
        >
          ABOUT US
        </h2>

        <h3
          class="text-xl sm:text-4xl lg:text-[1.45rem] lg:text-left lg:whitespace-nowrap px-4 lg:px-0 tracking-wide mt-6 lg:my-[2vw] w-full h-min lg:w-[36.5vw] lg:pt-[3vw]"
        >
          Lorem ipsum dolor sit amet, consectetur<br />adipiscing elit, sed do
          eiusmod tempor<br />incididunt ut labore et dolore magna<br />aliqua.
          Ut enim ad minim veniam, quis<br />nostrud exercitation ullamco
          laboris nisi<br />ut aliquip ex ea commodo consequat.<br />Duis aute
          irure dolor in reprehenderit in<br />voluptate velit esse cillum
          dolore eu<br />fugiat nulla pariatur. Excepteur sint<br />occaecat
          cupidatat non proident, sunt in<br />
          culpa qui officia deserunt mollit anim id<br />est laborum
        </h3>
        <ul
          class="text-xl sm:text-4xl lg:text-[1.45rem] lg:mt-0 mt-6 text-[4vw] lg:pt-[3vw] align-middle list-none grid place-items-center lg:block w-full lg:w-fit"
        >
          <li
            class="list-none before:inline-block before:bg-phone before:bg-no-repeat before:bg-center before:bg-contain before:w-[3.5vw] before:h-[3.5vw] sm:before:w-[2vw] sm:before:h-[2vw] list-outside text-left indent-[0.5vw] hover:before:animate-shakee"
          >
            <span class="align-top indent-[2vw] inline-block"
              >+01 24 56789 91011</span
            >
          </li>
          <li
            class="list-none before:inline-block before:bg-email before:bg-no-repeat before:bg-center before:bg-contain before:w-[3.5vw] before:h-[3.5vw] sm:before:w-[2vw] sm:before:h-[2vw] list-outside text-left indent-[0.5vw] hover:before:animate-shakee"
          >
            <span class="align-top indent-[2vw] inline-block"
              >work@myemail.com</span
            >
          </li>
          <li
            class="list-none before:inline-block before:bg-adr before:bg-no-repeat before:bg-center before:bg-contain b before:w-[3.5vw] before:h-[3.5vw] sm:before:w-[2vw] sm:before:h-[2vw] list-outside text-left indent-[0.5vw] hover:before:animate-shakee"
          >
            <span class="align-top indent-[2vw] inline-block">
              Your Adress Here</span
            >
          </li>
        </ul>
      </div>
    </intersect>
    <div
      class="flex lg:hidden items-center justify-center mt-8 w-full h-auto"
      :class="isObservable ? 'animate-fade-left ' : ''"
    >
      <img
        src="../assets/Landing-page/Home Design 4/Vector Smart Object (Double Click to Edit).png"
        alt=""
        class="block w-[70%] h-auto"
      />
    </div>
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