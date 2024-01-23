<template>
  <section
    class="lg:flex w-full h-auto items-center py-20 lg:pt-20 px-14 justify-center"
  >
    <div
      class="lg:flex hidden items-center justify-center h-full w-[55%]"
      :class="textIsObservable ? 'animate-fade-left animate-delay-200' : ''"
    >
      <img
        src="../assets/Landing-page/Home Design 2/Vector Smart Object (Double Click to Edit).png"
        alt=""
        class="block w-[85%] max-w-xl h-auto"
      />
    </div>

    <intersect
      @enter="textIsObservable = true"
      @leave="textIsObservable = false"
    >
      <div
        class="text-white lg:w-[45%] flex-col h-96"
        :class="textIsObservable ? 'animate-fade-left animate-delay-200' : ''"
      >
        <div class="lg:mb-14 mb-6 lg:w-fit h-fit">
          <h2
            class="font-['Audiowide'] lg:leading-normal lg:text-left leading-none block lg:whitespace-nowrap text-[2.5rem] md:text-[2.95rem] tracking-wide"
          >
            SMART HOME
          </h2>
          <h3
            class="text-3xl md:text-[2.1rem] lg:text-left block whitespace-nowrap font-medium tracking-wide"
          >
            security System
          </h3>
        </div>

        <h4
          class="text-xl sm:text-4xl lg:text-[1.45rem] lg:text-left block lg:whitespace-nowrap"
        >
          “Lorem ipsum dolor sit amet,<br />consectetur adipiscing elit,<br />
          sed do eiusmod tempor incididunt<br />ut labore et dolore magna
          aliqua.”
        </h4>
      </div>
    </intersect>
    <div
      class="lg:hidden flex items-center mt-8 justify-center h-auto w-full"
      :class="textIsObservable ? 'animate-fade-left animate-delay-200' : ''"
    >
      <img
        src="../assets/Landing-page/Home Design 2/Vector Smart Object (Double Click to Edit).png"
        alt=""
        class="block w-[85%] h-auto"
      />
    </div>
  </section>
</template>

<script>
import intersect from "vue-intersect";
export default {
  data() {
    return {
      textIsObservable: false,
      imageIsObservable: false,
    };
  },
  components: {
    intersect,
  },
};
</script>

<style>
</style>