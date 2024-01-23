<template class="grod place-items-center">
  <section
    class="w-full static overflow-hidden py-20 lg:py-0 lg:px-0 md:mt-[4vw] flex h-max items-center bg-contain bg-no-repeat justify-center"
  >
    <intersect @enter="isObservable = true" @leave="isObservable = false">
      <div
        class="lg:flex flex-column justify-around lg:my-[8vw] md:px-8 z-10 items-center text-white w-full"
      >
        <div
          class="space-y-4 mx-auto z-10 lg:w-max lg:grid place-content-center gap-y-[1vw] sm:gap-y-1 lg:gap-y-[4vw] grid-rows-[20vh,auto] transition-all ease-in duration-500"
          :class="
            isObservable ? '' : 'lg:translate-y-[100%] lg:opacity-0 lg:blur-md'
          "
        >
          <img
            class="w-[40%] block h-auto mx-auto my-auto"
            src="../assets/Landing-page/Shapes/Shape-3.png"
            alt=""
          />
          <div class="space-y-[1vw]">
            <h1 class="md:text-3xl text-[4vw] font-semibold tracking-wide">
              SECURITY SYSTEM
            </h1>
            <h3 class="lg:text-xl md:text-4xl px-4 text-xl">
              Lorem ipsum dolor sit amet,<br />consectetur adipiscing elit,<br />
              sed do eiusmod tempor incididunt
            </h3>
          </div>
        </div>
        <div
          class="space-y-4 mx-auto z-10 lg:w-max my-[20%] lg:my-0 lg:grid place-content-center gap-y-[1vw] sm:gap-y-1 lg:gap-y-[3vw] grid-rows-[20vh,auto] transition-all ease-in duration-500 delay-200"
          :class="
            isObservable ? '' : 'lg:translate-y-[100%] lg:opacity-0 lg:blur-md'
          "
        >
          <img
            class="w-[40%] block h-auto mx-auto my-auto"
            src="../assets/Landing-page/Shapes/Shape-2.png"
            alt=""
          />
          <div class="space-y-[1vw]">
            <h1 class="md:text-3xl text-[4vw] font-semibold tracking-wide">
              SMART LAMP
            </h1>
            <h3 class="lg:text-xl md:text-4xl px-4 text-xl">
              Lorem ipsum dolor sit amet,<br />consectetur adipiscing elit,<br />
              sed do eiusmod tempor incididunt
            </h3>
          </div>
        </div>

        <div
          class="space-y-4 mx-auto z-10 lg:w-max mt-[20%] lg:my-0 lg:grid place-content-center gap-y-[1vw] sm:gap-y-1 lg:gap-y-[3vw] grid-rows-[20vh,auto] transition-all ease-in duration-500 delay-[400ms]"
          :class="
            isObservable ? '' : 'lg:translate-y-[100%] lg:opacity-0 lg:blur-md'
          "
        >
          <img
            class="w-[40%] block h-auto mx-auto my-auto"
            src="../assets/Landing-page/Shapes/Shape-1.png"
            alt=""
          />
          <div class="space-y-[1vw]">
            <h1 class="md:text-3xl text-[4vw] font-semibold tracking-wide">
              CCTV CONTROL
            </h1>
            <h3 class="lg:text-xl md:text-4xl px-4 text-xl">
              Lorem ipsum dolor sit amet,<br />consectetur adipiscing elit,<br />
              sed do eiusmod tempor incididunt
            </h3>
          </div>
        </div>
      </div>
    </intersect>

    <img
      src="../assets/Landing-page/Backgrounds/Group 2 card/Rounded Rectangle.png"
      alt=""
      class="w-full lg:block hidden absolute z-0"
    />
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
  components: { intersect },
};
</script>

<style>
</style>