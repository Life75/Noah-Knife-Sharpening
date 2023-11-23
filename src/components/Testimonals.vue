<template>
  <div class="text-left">
    <P class="font-bold text-7xl text-center pb-7 ">Testimonals</P>
    <span class="md:flex md:space-x-10 ">
    <ReviewCards
      description="Noah is excellent! My knives have never been sharper and he came to
                  me! I 1000% endorse his work and fair prices. If you need a knife
                  sharpener he should be #1 on your list."
      :stars="5"
      name="Zach H"
      class="mb-4"
    />

    <ReviewCards
      description= "I just used this service. I'm very very satisfied. Noah's very nice
                    and professional. He left my Shikomizue razor sharp and even notified
                    me of a problem with my cane sword. Reasonably priced and
                    professional. I will use him again."
      :stars="5"
      name="Justice F"
      class="mb-4"
    />

    <ReviewCards
      description= "Incredible service. I dropped off 16 Wustoff knives to Noah earlier
                    today and he had them done within 2 hours. These knives have never
                    been sharper! Very quick, very efficient, and very well priced. I
                    would recommend this service to anyone in the Pinellas area who needs
                    their blades honed."
      :stars="5"
      name="Josh E"
      class="mb-4"
    />
  </span>


    <div class="flex justify-center align-middle space-x-6 pt-8 text-xl font-medium">
      <button
        class="bg-white hover:bg-gray-200 text-gray-800 font-semibold py-2 px-4 border border-gray-400 rounded shadow buttonAnimation"
      >
        Write a Review
      </button>

      <button
        class="bg-white hover:bg-gray-200 text-gray-800 font-semibold py-2 px-4 border border-gray-400 rounded shadow buttonAnimation"
      >
        Read More
      </button>
    </div>
  </div>
</template>

<script setup lang="ts">
import ReviewCards from "./ReviewCards.vue";
</script>

<style>
.review-text {
  @apply leading-normal  text-base font-bold text-lg;
}

.buttonAnimation:hover {
  animation-name: up-movement;
  animation-duration: 0.2s;
  animation-fill-mode: forwards;
  box-shadow: 0 0 50px 15px #48abe0;

  @apply shadow-lg  hover:bg-gray-200;
}

@keyframes up-movement {
  from {
  }
  to {
    transform: translateY(-6px);
  }
}
</style>
