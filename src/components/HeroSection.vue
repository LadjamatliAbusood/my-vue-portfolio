<template>
  <section class="relative w-full" data-aos="zoom-in-up">
    <!-- <div class="absolute top-0 inset-x-0 h-64 flex items-start">
      <div
        class="h-24 w-2/3 bg-gradient-to-br from-[#570cac] blur-2xl invisible opacity-40"
      ></div>
      <div
        class="h-20 w-3/5 bg-gradient-to-r from-[#670ccf] opacity-40 blur-2xl"
      ></div>
    </div> -->

    <div
      class="w-full px-5 sm:px-8 md:px-12 lg:px-8 max-w-screen-lg lg:max-w-screen-xl mx-auto relative"
    >
      <div
        class="grid lg:grid-cols-2 gap-10 xl:gap-14 relative pt-1 lg:max-w-none max-w-2xl md:max-w-3xl mx-auto"
      >
        <div class="lg:py-6">
          <div class="text-center lg:text-left">
            <h1
              class="pt-4 text-gray-600 font-bold text-4xl md:text-5xl lg:text-6xl"
            >
              Hi, I'm AJ 😁
            </h1>
          </div>
          <p
            class="text-gray-600 pt-8 text-center lg:text-left mx-auto max-w-xl"
          >
            As a Full Stack Developer, I specialize in building android app and
            deploying dynamic, responsive websites. Here's a link to my v1
            portfolio
            <a
              href="https://ladjamatliabusood.github.io/AJLPortfolio/"
              class="text-primary hover:text-primary/80"
              >@ajladjamatli</a
            >
          </p>
          <div
            class="flex items-center gap-3 pt-9 flex-col sm:flex-row sm:w-max sm:mx-auto lg:mx-0"
          >
            <button
              class="px-6 md:px-7 py-3 rounded-full relative group w-full sm:w-max flex justify-center"
            >
              <span
                class="absolute inset-0 rounded-3xl group-hover:scale-105 origin-center transition-all ease-in-out bg-primary border-2 border-transparent"
              ></span>
              <div class="svg-container mr-2">
                <div class="download-loader" style="width: 25px; height: 25px">
                  <img
                    src="@/assets/coffee.png"
                    alt=""
                    class="filter invert brightness-0"
                  />
                </div>
              </div>
              <span class="relative flex items-center justify-center text-white"
                ><a href="https://buymeacoffee.com/ajladjamatli"
                  >Buy me a coffee</a
                ></span
              >
            </button>
            <button
              class="border border-primary px-6 md:px-7 py-3 rounded-full relative group w-full sm:w-max flex justify-center"
            >
              <div
                class="hover:scale-105 transition-all ease-in-out flex justify-center items-center relative"
              >
                <div class="svg-container">
                  <div
                    class="download-loader"
                    style="width: 25px; height: 25px"
                  >
                    <img
                      src="@/assets/dwnld.png"
                      alt=""
                      class="filter invert brightness-50"
                    />
                  </div>
                </div>
                <a
                  href="https://drive.google.com/file/d/1USdiNA0GQvNJUX1X7qJl6x8jCVWYiNSU/view?usp=drive_link"
                  class="pl-2 text-primary"
                  >Resume</a
                >
              </div>
            </button>
          </div>
        </div>
        <div class="lg:h-full md:flex">
          <div
            class="flex w-full h-96 min-h-[24rem] lg:min-h-[none] lg:w-full lg:h-full items-center relative"
          >
            <div
              class="absolute z-0 top-1/2 -translate-y-1/2 w-5/6 right-0 h-[calc(80%+20px)] bg-gradient-to-tr opacity-25 from-[#570cac] to-primary blur-2xl"
            ></div>
            <div
              class="absolute h-full z-10 p-2 -translate-y-1/2 top-1/2 lg:right-3 md:right-40 sm:right-16 rounded-full shadow-lg border border-primary"
            >
              <img
                src="@/assets/img3.png"
                alt="Hero pic"
                width="500"
                height="auto"
                loading="lazy"
                class="w-full h-full rounded-full object-cover"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import AOS from "aos";
import "aos/dist/aos.css";
AOS.init();
</script>
