<template>
  <section class="text-white py-20 lg:py-0 overflow-hidden">
    <h1
      class="text-[2.5rem] lg:text-[3.2rem] sm:tracking-widex font-semibold sm:py-[6vw] lg:mb-0 mb-6"
    >
      SECURITY MODE TYPE
    </h1>
    <intersect
      @enter="cardsAreObservable = true"
      @leave="cardsAreObservable = false"
    >
      <div
        class="lg:flex flex-column sm:grid col-span-full grid-cols-2 mb-6 items-center justify-around"
      >
        <Tilt parallax="true">
          <div
            class="relative z-0 grid place-items-center bg-card-purple-rectangle bg-center h-[150vw] w-full sm:h-[80vw] lg:h-[50vw] lg:w-[30vw] bg-no-repeat bg-cover transition-all ease-in duration-300"
            :class="
              cardsAreObservable
                ? ''
                : 'opacity-0 translate-x-[-100%] blur-lg animate-delay-500'
            "
          >
            <div
              class="z-10 w-full h-fit grid place-items-center grid-rows-[60%,auto,auto]"
            >
              <div class="flex items-center justify-center w-[75%]">
                <img
                  src="../assets/Landing-page/Cards Home Designs/png1.png"
                  alt=""
                  class="h-auto place w-full block"
                />
              </div>

              <div>
                <h1
                  class="font-['Audiowide'] sm:text-[4vw] text-[6vw] lg:text-[2.5vw]"
                >
                  TYPE A
                </h1>
                <h3 class="text-left text-[4vw] sm:text-[2vw] lg:text-[1.25vw]">
                  Lorem ipsum dolor sit amet,<br />consectetur adipiscing
                  elit,<br />
                  sed do eiusmod tempor incididunt
                </h3>
              </div>
              <button
                class="border-solid border border-white text-[3.5vw] sm:text-[2vw] sm:py-[1vw] lg:text-[1.2vw] lg:px-[2.5vw] px-[8vw] py-[1vw] lg:py-[0.3vw] my-6 rounded-full hover:shadow-fuchsia-700 hover:scale-110 transition-all ease-in duration-200 shadow-lg"
              >
                See More
              </button>
            </div>
          </div>
        </Tilt>

        <Tilt parallax="true">
          <div
            class="relative z-0 grid place-items-center sm:h-[80vw] bg-card-purple-rectangle bg-center h-[150vw] w-full lg:h-[50vw] lg:w-[30vw] bg-no-repeat bg-cover transition-all ease-in duration-300 delay-200"
            :class="
              cardsAreObservable
                ? ''
                : 'opacity-0 translate-x-[-100%] blur-lg animate-delay-500'
            "
          >
            <div
              class="z-10 w-full h-fit grid place-items-center grid-rows-[60%,auto,auto]"
            >
              <div class="flex items-center justify-center w-[75%]">
                <img
                  src="../assets/Landing-page/Cards Home Designs/png2.png"
                  alt=""
                  class="h-auto place w-full block"
                />
              </div>
              <div>
                <h1
                  class="font-['Audiowide'] sm:text-[4vw] text-[6vw] lg:text-[2.5vw]"
                >
                  TYPE B
                </h1>
                <h3 class="text-left text-[4vw] sm:text-[2vw] lg:text-[1.25vw]">
                  Lorem ipsum dolor sit amet,<br />consectetur adipiscing
                  elit,<br />
                  sed do eiusmod tempor incididunt
                </h3>
              </div>
              <button
                class="border-solid border border-white text-[3.5vw] sm:text-[2vw] sm:py-[1vw] lg:text-[1.2vw] lg:px-[2.5vw] px-[8vw] py-[1vw] lg:py-[0.3vw] my-6 rounded-full hover:shadow-fuchsia-700 hover:scale-110 transition-all ease-in duration-200 shadow-lg"
              >
                See More
              </button>
            </div>
          </div>
        </Tilt>

        <Tilt
          parallax="true"
          class="sm:col-span-2 sm:w-fit sm:h-fit sm:place-self-center"
        >
          <div
            class="relative z-0 grid place-items-center sm:h-[80vw] bg-card-purple-rectangle bg-center h-[150vw] w-full lg:h-[50vw] lg:w-[30vw] bg-no-repeat bg-cover transition-all ease-in duration-300 delay-[400ms]"
            :class="
              cardsAreObservable
                ? ''
                : 'opacity-0 translate-x-[-100%] blur-lg animate-delay-500'
            "
          >
            <div
              class="z-10 w-full h-fit grid place-items-center grid-rows-[60%,auto,auto]"
            >
              <div class="flex items-center justify-center w-[75%]">
                <img
                  src="../assets/Landing-page/Cards Home Designs/png3.png"
                  alt=""
                  class="h-auto place w-full block"
                />
              </div>

              <div>
                <h1
                  class="font-['Audiowide'] sm:text-[4vw] text-[6vw] lg:text-[2.5vw]"
                >
                  TYPE C
                </h1>
                <h3 class="text-left text-[4vw] sm:text-[2vw] lg:text-[1.25vw]">
                  Lorem ipsum dolor sit amet,<br />consectetur adipiscing
                  elit,<br />
                  sed do eiusmod tempor incididunt
                </h3>
              </div>
              <button
                class="border-solid border border-white text-[3.5vw] sm:text-[2vw] sm:py-[1vw] lg:text-[1.2vw] lg:px-[2.5vw] px-[8vw] py-[1vw] lg:py-[0.3vw] my-6 rounded-full hover:shadow-fuchsia-700 hover:scale-110 transition-all ease-in duration-200 shadow-lg"
              >
                See More
              </button>
            </div>
          </div>
        </Tilt>
      </div>
    </intersect>

    <intersect
      @enter="textIsObservable = true"
      @leave="textIsObservable = false"
    >
      <h3
        class="text-xl sm:text-4xl lg:text-[1.45rem] tracking-wide px-4 lg:px-0 lg:my-[2vw] transition-all ease-in duration-500"
        :class="textIsObservable ? 'animate-fade-down' : ''"
      >
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut<br />
        labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
        exercitation ullamco<br />
        laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
        in reprehenderit in
      </h3>
    </intersect>
  </section>
</template>

<script>
import intersect from "vue-intersect";
import Tilt from "vanilla-tilt-vue";
import { Carousel3d, Slide } from "vue-carousel-3d";
export default {
  data() {
    return {
      textIsObservable: false,
      cardsAreObservable: false,
    };
  },
  components: {
    intersect,
    Tilt,
    Carousel3d,
    Slide,
  },
  methods: {},
};
</script>

<style>
</style>