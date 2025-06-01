<template>
  <section class="text-gray-600 mt-20" id="services ">
    <div class="px-4 xl:pl-16">
      <h2 class="text-4xl font-bold mb-4">Services</h2>
    </div>
    <div
      class="py-8 xl:px px-4 sm:py-16 grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:gap-10 md:pt-12 lg:grid-cols-3"
    >
      <div
        v-for="service in services"
        :key="service.id"
        data-aos="fade-up"
        class="px-8 py-12 rounded-xl bg-[#fdfdfd] shadow-lg border border-[gray-200]"
      >
        <div class="mx-auto h-24 text-center xl:h-28 xl:w-28">
          <div>
            <img
              :src="service.icon"
              alt="service icon"
              class="filter invert brightness-50"
            />
          </div>
        </div>
        <div class="text-center">
          <h3
            class="pt-8 text-lg font-semibold uppercase text-gray-600 lg:text-xl"
          >
            {{ service.name }}
          </h3>
          <p
            class="text-gray pt-4 text-sm group-hover:text-gray-900 md:text-base"
          >
            {{ service.description }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
const services = ref([
  {
    id: 1,
    icon: new URL("@/assets/res.png", import.meta.url).href,
    name: "WEB DEVELOPEMENT",
    description:
      "Building responsive and dynamic websites using modern frameworks and technologies.",
  },
  {
    id: 2,
    icon: new URL("@/assets/android.png", import.meta.url).href,
    name: "Mobile DEVELOPEMENT",
    description:
      "Creating mobile applications for Android with seamless user experiences.",
  },
  {
    id: 3,
    icon: new URL("@/assets/techsupport.png", import.meta.url).href,
    name: "Technical Support",
    description:
      "Knowledgeable in troubleshooting computer hardware, software, and network issues.",
  },
  {
    id: 4,
    icon: new URL("@/assets/computer.png", import.meta.url).href,
    name: "Computer Literate",
    description:
      "Have knowledge in Microsoft Office such as Microsoft Word, Excel and Power Point Presentation.",
  },
  {
    id: 5,
    icon: new URL("@/assets/ps.png", import.meta.url).href,
    name: "Image Editing",
    description:
      "Photo retouching, manipulation, and enhancement using advanced editing tools.",
  },
  {
    id: 6,
    icon: new URL("@/assets/video.png", import.meta.url).href,
    name: "Video Editing",
    description: "Video editing, color correction to enhance your content.",
  },
]);
</script>
