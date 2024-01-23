<template>
  <section
    class="lg:flex w-full h-auto py-20 px-14 items-center justify-center"
  >
    <intersect
      @enter="isObservable = true"
      @leave="isObservable = false"
      class="w-max h-max"
    >
      <div
        class="text-white flex items-center justify-center h-full z-10 lg:w-[50%]"
        :class="isObservable ? 'animate-fade-right' : ''"
      >
        <div class="w-fit h-fit">
          <h1
            class="font-[Audiowide] whitespace-nowrap lg:text-left text-5xl md:text-[5.5rem] tracking-wider leading-none"
          >
            FUTURE<br />
            IS NOW
          </h1>
          <h2
            class="text-[2.5rem] md:text-[2.95rem] lg:text-left mt-6 lg:mt-0 mb-6 whitespace-nowrap font-medium leading-none tracking-widest"
          >
            SMART HOME
          </h2>

          <h4
            class="text-xl sm:text-4xl lg:text-[1.45rem] lg:px-0 px-4 lg:text-left lg:leading-tight pb-10 whitespace-nowrap"
          >
            Lorem ipsum dolor sit amet,<br />consectetur adipiscing elit, sed do
          </h4>

          <button
            class="border-solid border border-white ml-0 lg:float-left text-xl sm:text-4xl lg:text-2xl px-[5.5vw] py-[0.5vw] md:py-2 md:px-16 rounded-full hover:shadow-fuchsia-700 hover:scale-110 transition-all ease-in duration-200 shadow-lg"
          >
            See More
          </button>
        </div>
      </div>
    </intersect>
    <div
      class="flex items-center pt-8 lg:pt-0 justify-center h-full lg:w-[50%]"
      :class="isObservable ? ' animate-fade-right' : ''"
    >
      <img
        src="../assets/Landing-page/Home Design/Vector Smart Object (Double Click to Edit).png"
        alt=""
        class="block w-[85%] max-w-xl h-auto"
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