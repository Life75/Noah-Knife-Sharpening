<template>
  <div id="instructions" class="py-5 rounded shadow-xl border-2 border-gray-400  bg-[#353332] ">
    
    <div class="">
      <p class="text-center text-5xl font-extrabold pt-1.5">By Appointment Only</p>
    </div>
    <div class="justify-center align-middle m-7">
      <p class="text-2xl text-center">
        I provide a mobile and drop-off sharpening service for a variety of blades and
        tools like kitchen cutlery, scissors, garden tools, hatchets and axes, swords,
        pocket and hunting knives, lawnmower blades, and more.
      </p>
      <div class="text-center text-3xl py-10">
        <p class="text-4xl pt-5 font-bold pb-2">Prices</p>
        <span class="font-bold">
          <p>$1 per inch with a minimum of $5</p>
          <p>$1.5 per for serrated</p>
          <p>$5 for basic scissors</p>
          <p>$5 for tip repair (large broken tip)</p>
          <p>Other items subject to price discussion</p>
          <p class="">*If you are a restaurant, ask about special deals*</p>
        </span>
      </div>
      <p class="text-center text-4xl pt-8 pb-6 font-bold">Options for services</p>
      <span class="lg:flex justify-center align-middle  md:space-y-0 md:space-x-4 space-x-0 space-y-5  ">
        <v-card class=" text-xl" color="#cccccc" max-width="420"  min-width="300"  min-height="450" max-height="400"
             >
             <template v-slot:prepend>
                <v-icon icon="mdi-car" ></v-icon>
             </template>
             <template v-slot:title>
             <p class="text-3xl font-bold">Mobile</p>
             </template>
            <v-card-text>
              <p class="text-2xl text-gray-700">
              For mobile, I will come out to you with my equipment and sharpen your knives while you're in the comfort of
              your own home.
            </p>
            <p class="mt-2 text-2xl text-gray-700 text-left">
              Mobile Service For Knives: $15 fee. $3 fee per mile after 10 mi. Call or text the number provided for
              details and setting up an appointment.

            </p>
            
            </v-card-text>
          </v-card>
      
        <v-card class=" text-xl  cursor-pointer " color="#cccccc"  max-width="420"  min-width="300"  min-height="450" link href="https://youtube.com/shorts/2lnKg-dXgIA?feature=share" append-icon="mdi-help-circle"
             >
             <template v-slot:prepend>
                <v-icon icon="mdi-package" ></v-icon>
             </template>
             <template v-slot:title>
                <p class="text-3xl font-bold">Drop Off</p>
             </template>
            <v-card-text>
              <p class="mt-2 text-2xl text-gray-700 text-left ">
              For drop off services
              schedule a time that is best for you to come and drop off your items in one of the locker slots on the porch
              of my residence. Please do not knock on the door. There will be instructions on the locker to guide you.
            </p>
            </v-card-text>
          </v-card>
    
          <v-card class=" text-xl cursor-pointer" color="#cccccc" max-width="420"  min-width="300"  min-height="400" max-height="450" link href="https://youtube.com/shorts/2lnKg-dXgIA?feature=share" append-icon="mdi-help-circle"
             >
             <template v-slot:prepend>
                <v-icon icon="mdi-package" ></v-icon>
             </template>
             <template v-slot:title>
             <p class="text-3xl font-bold text-wrap ">Drop Off: Restoration</p>
             </template>
            <v-card-text>
              <p class="mt-2 text-2xl text-gray-700 text-left ">
                Full derust, repair, cleaning, and polish for damaged blades. 
              </p>
              <p class="mt-2 text-2xl text-gray-700 text-left ">
                • No handle structure repairs, only metal cleaning and polishing. 
              </p>
              <p class="mt-2 text-2xl text-gray-700 text-left text-wrap ">
                • $25 an hour (can take anywhere between 1-5 hours depending on damage)
            </p>
            </v-card-text>
          </v-card>
        <div>

        </div>
      </span>
    </div>
  
  </div>
</template>

<script setup lang="ts">

</script>
