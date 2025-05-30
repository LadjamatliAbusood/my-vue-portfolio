<template>
  <section class="text-white mt-18" id="skills">
    <div class="absolute right-0 top-[110rem] h-full w-full justify-end">
      <span class="flex opacity-20">
        <span class="w-16 h-32 rounded-l-full flex bg-primary blur-2xl"></span>
        <span
          class="w-16 h-32 rounded-r-full flex bg-[#f88fc2] blur-2xl mt-14"
        ></span>
      </span>
    </div>
    <div
      class="md:grid md:grid-cols-2 gap-8 items-center py-8 px-4 xl:gap-16 xl:px-16"
    >
      <!-- Left Side -->
      <div class="mt-4 md:mt-0 text-left flex flex-col z-10 h-full w-[80%]">
        <h2 class="text-4xl font-bold text-gray-600 text-left mb-4">
          <span
            class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary"
            >Skills</span
          >
        </h2>
        <div class="mt-8" v-for="skills in Skills" :key="skills.id">
          <div class="flex items-end justify-between" data-aos="fade-right">
            <h4 class="font-semibold uppercase text-gray-600 text-lg">
              {{ skills.name }}
            </h4>
            <h3 class="text-2xl font-bold text-gray-600">{{ skills.width }}</h3>
          </div>
          <div class="mt-2 h-1 w-full bg-[#131d30] rounded-full">
            <div
              class="h-1 rounded-full bg-primary"
              :style="`width :${skills.width}`"
            ></div>
          </div>
        </div>
      </div>
      <!-- Right Side -->
      <div data-aos="flip-left">
        <h2
          class="text-4xl font-bold text-gray-600 text-left mb-8 md:text-center md:mt-0 mt-8"
        >
          <span
            class="text-transparent bg-clip-text bg-gradient-to-r from-secondary to-primary"
            >Experience</span
          >
        </h2>
        <div class="space-y-8 py-8" data-aos="fade-left">
          <div
            v-for="element in Experience"
            :key="element.id"
            class="flex items-center rounded-xl p-4 bg-[#fdfdfd] shadow-lg border border-[gray-200]"
          >
            <div class="w-1/4">
              <img
                :src="element.icon"
                alt="service icon"
                class="filter invert brightness-50"
              />
            </div>
            <div class="w-3/4 pl-4">
              <h3
                class="text-2xl font-semibold uppercase text-trasparent bg-clip-text text-gray-600"
              >
                {{ element.role }}
              </h3>
              <p class="text-gray-600">{{ element.company }}</p>
              <p class="text-gray-600">{{ element.address }}</p>
              <p class="text-gray-600">{{ element.date }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
const Skills = ref([
  {
    id: 1,
    name: "HTML, JS & CSS",
    width: "75%",
  },
  {
    id: 2,
    name: "Java",
    width: "55%",
  },
  {
    id: 3,
    name: "PHP",
    width: "65%",
  },
  {
    id: 4,
    name: "Mysql",
    width: "55%",
  },
]);

const Experience = ref([
  {
    id: 1,
    icon: new URL("@/assets/hospital.png", import.meta.url).href,
    role: "Jr Programmer",
    company: "West Metro Medical Center",
    address: "Zamboanga City",
    date: "April 2024 - August 2024",
  },
  {
    id: 2,
    icon: new URL("@/assets/cityhall.png", import.meta.url).href,
    role: "Records Division",
    company: "Sangguniang Panlungsod ng Zamboanga",
    address: "Zamboanga City",
    date: "July 2023 - December 2023",
  },
]);
</script>
