<template>
  <section
    class="text-white bg-spec pb-[5vw] flex-col lg:mt-0 mt-20 justify-center overflow-hidden"
  >
    <h1
      class="text-[2.5rem] lg:text-[3vw] leading-none lg:whitespace-nowrap font-bold md:tracking-widex z-10 mt-[2vw] py-[5vw]"
    >
      Check what your house can do for you
    </h1>

    <intersect @enter="isObservable = true" @leave="isObservable = false">
      <div
        class="grid grid-rows-3 lg:grid-rows-1 lg:grid-cols-3 z-10 place-items-center my-[6vw] lg:my-0 md:mx-[4vw] gap-[5%] md:gap-[2%]"
      >
        <Tilt parallax="true" glare="true" class="w-[80%] md:w-full">
          <img
            src="../assets/Landing-page/Images/v2/img1.png"
            alt=""
            class="block w-full z-10 drop-shadow-spec"
            :class="isObservable ? 'animate-rotate-y' : ''"
          />
        </Tilt>

        <Tilt parallax="true" glare="true" class="w-[80%] md:w-full">
          <img
            src="../assets/Landing-page/Images/v2/img2.png"
            alt=""
            class="block w-full z-10 drop-shadow-spec"
            :class="isObservable ? 'animate-rotate-y animate-delay-150' : ''"
          />
        </Tilt>

        <Tilt parallax="true" glare="true" class="w-[80%] md:w-full">
          <img
            src="../assets/Landing-page/Images/v2/img3.png"
            alt=""
            class="block w-full z-10 drop-shadow-spec"
            :class="isObservable ? 'animate-rotate-y animate-delay-300' : ''"
          />
        </Tilt>
      </div>
    </intersect>
  </section>
</template>

<script>
import intersect from "vue-intersect";
import Tilt from "vanilla-tilt-vue";

export default {
  data() {
    return {
      isObservable: false,
    };
  },
  components: {
    intersect,
    Tilt,
  },
};
</script>

<style>
.bg-spec {
  filter: drop-shadow(0px 15px 25px rgba(0, 0, 0, 0.2));
  background-image: linear-gradient(
    0deg,
    rgba(151, 14, 129, 0.9999999999999999) 0%,
    rgba(248, 236, 245, 0.2) 100%
  );
  border: 0.3vw solid rgba(248, 236, 245, 0.2);
  border-right: none;
  border-left: none;
}
.carousel-3d-3d-Slide {
  width: fit-content;
  height: fit-content;
}
</style>