<template>
  <section class="text-white mt-18" id="about">
    <div class="absolute z-0 top-[93rem] inset-x-0 h-64 flex items-start">
        <div class="h-24 w-64 bg-gradient-to-br from-primary via-secondary blur-2xl to-[#570cac] opacity-20"></div>
    </div>
    <div class="md:grid md:grid-cols-2 gap-8 items-center py-8 px-4 xl:gap-16 sm:py-16 xl:px-16 z-1">
        <!-- Left side -->
        <div data-aos="flip-right">
            <h2 class="text-4xl font-bold text-white text-left mb-8">My Education</h2>
            <div class="space-y-8 py-8">
                <div v-for="element in education" :key="element.id"
                class="flex items-center md:w-[80%] w-full rounded-xl bg-[#111a3e] shadow-lg border boder-[#1f1641]">
                <div class="w-1/4">
                    <img src="@/assets/grad.png" alt="graduation">
                </div>
                <div class="w-3/4 pl-4">
                    <h3 class="text-2xl font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary lg:text-xl">
                        {{ element.School }}
                    </h3>
                    <p class="text-white">{{ element.Program }}</p>
                    <p class="text-white">{{ element.year }}</p>

                </div>
            </div>
            </div>

        </div>
    <!-- Right side -->
     <div class="mt-4 md:mt-0 text-left flex flex-col z-10 h-full" data-aos="flip-right">
        <h2 class="text-4xl font-bold text-white md:text-center text-left mb-4">More
            <span class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">About</span> Me
        </h2>
        <p class="text-gray-300 pt-8 text-center lg:text-left mx-auto max-w-xl">
            I like diving into the latest trends in technology. In my free time, I enjoy playing video games, watching K-dramas, and exploring new innovations. 
            Whether watching a captivating series, or staying updated on cutting-edge tech, I'm always eager to learn and experience something new.
         </p>
         <div class="grid grid-cols-3 gap-4 max-w-lg pt-8">
            <!-- <div class="text-center rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641] p-3">
                <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">+200</h3>
                <p class="text-sm sm:text-base text-gray-300">Happy Client</p>
            </div>

            <div class="text-center rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641] p-3">
                <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">+200</h3>
                <p class="text-sm sm:text-base text-gray-300">Happy Client</p>
            </div> -->
         
          
            <div class="text-center rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641] p-3">
                <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">+3</h3>
                <p class="text-sm sm:text-base text-gray-300">Experience</p>
            </div>
         </div>

         
        
         
     </div>
        
    </div>

  </section>
</template>

<script setup>
import {ref} from 'vue';
const education = ref([
    {
        id:1,
        School: 'Western Mindanao State University',
        Program: 'Information Technology',
        year: '2023'

    },

])

</script>

