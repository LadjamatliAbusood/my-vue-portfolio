<template>
  <section class="text-white mt-20" id="contact">
    <h2 class="text-4xl font-bold text-gray-600 text-center mb-4 px-4 xl:pl-16">
      Let's Connect
    </h2>

    <div class="container p-5 flex justify-center">
      <div>
        <div
          class="grid md:grid-cols-4 gap-4 relative px-4 xl:px-16 mt-8"
          data-aos="zoom-in-up"
        >
          <div class="flex items-center space-x-4">
            <div class="p-2">
              <img
                src="@/assets/gmail.png"
                alt="new-post"
                class="filter invert brightness-100 w-9"
              />
            </div>
            <div class="text-gray-600">
              <h4>Email</h4>
              <p>ladjamatli5@gmail.com</p>
            </div>
          </div>

          <div class="flex items-center space-x-4">
            <div class="p-2">
              <img
                src="@/assets/phone.png"
                alt="phone"
                class="filter invert brightness-100 w-9"
              />
            </div>
            <div class="text-gray-600">
              <h4>Phone</h4>
              <p>+63 962 450 1604</p>
            </div>
          </div>

          <div class="flex items-center space-x-4">
            <div class="p-2">
              <img
                src="@/assets/linked.png"
                alt="linkedin"
                class="filter invert brightness-100 w-9"
              />
            </div>
            <div class="text-gray-600">
              <h4>LinkedIn</h4>
              <a
                href="https://www.linkedin.com/in/ajladjamatli/"
                class="text-blue-400 underline"
                >Abusood Ladjamatli</a
              >
            </div>
          </div>

          <div class="flex items-center space-x-4">
            <div class="p-2">
              <img
                src="@/assets/ig.png"
                alt="linkedin"
                class="filter invert brightness-100 w-9"
              />
            </div>
            <div class="text-gray-600">
              <h4>Instagram</h4>
              <a
                href="https://www.instagram.com/itshkn199x/"
                class="text-blue-400 underline"
                >AJ Ladjamatli</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Old -->
    <!-- 
    <div
      class="grid md:grid-cols-2 gap-4 relative px-4 xl:px-16 mt-8"
      data-aos="zoom-in-up"
    >
      <div>
        <div
          class="grid md:grid-cols-2 gap-4 relative px-4 xl:px-16 mt-8"
          data-aos="zoom-in-up"
        >
          <div class="flex items-center space-x-4">
            <div
              class="p-2 bg-[#111a3e] w-[50px] h-[46px] flex justify-center items-center rounded-full border border-[#111a3e] backdrop-blur-md"
            >
              <img src="@/assets/gmail.png" alt="new-post" class="w-6" />
            </div>
            <div class="text-white">
              <h4>Email</h4>
              <p>ladjamatli5@gmail.com</p>
            </div>
          </div>

          <div class="flex items-center space-x-4">
            <div
              class="p-2 bg-[#111a3e] w-[50px] h-[46px] flex justify-center items-center rounded-full border border-[#111a3e] backdrop-blur-md"
            >
              <img src="@/assets/phone.png" alt="phone" class="w-6" />
            </div>
            <div class="text-white">
              <h4>Phone</h4>
              <p>+63 962 450 1604</p>
            </div>
          </div>

          <div class="flex items-center space-x-4">
            <div
              class="p-2 bg-[#111a3e] w-[50px] h-[46px] flex justify-center items-center rounded-full border border-[#111a3e] backdrop-blur-md"
            >
              <img src="@/assets/phone.png" alt="linkedin" class="w-6" />
            </div>
            <div class="text-white">
              <h4>LinkedIn</h4>
              <a
                href="https://www.linkedin.com/in/ajladjamatli/"
                class="text-blue-400 underline"
                >Abusood Ladjamatli</a
              >
            </div>
          </div>
        </div>
      </div>

      <div
        style="
          background: #111a3e;
          width: 100%;
          height: 100%;
          border-radius: 20px;
          overflow: hidden;
          border: 1px solid #111a3e;
          backdrop-filter: blur(9px);
          -webkit-backdrop-filter: blur(9px);
        "
      >
        <form class="flex flex-col p-2" data-aos="zoom-in-up">
          <div class="mb-6">
            <label for="email" class="text-white block mb-2 text-sm font-medium"
              >Email</label
            >
            <input
              type="email"
              id="email"
              class="bg-[#111827] placeholder:[#9CA2A9] text-gray-100 text-sm rounded-lg block w-full p-2.5"
              placeholder="email@gmail.com"
              name="email"
            />
          </div>
          <div class="mb-6">
            <label
              for="subject"
              class="text-white block mb-2 text-sm font-medium"
              >Subject</label
            >
            <input
              type="subject"
              id="subject"
              class="bg-[#111827] placeholder:[#9CA2A9] text-gray-100 text-sm rounded-lg block w-full p-2.5"
              placeholder="subject"
              name="subject"
            />
          </div>
          <div class="mb-6">
            <label
              for="message"
              class="text-white block mb-2 text-sm font-medium"
              >Message</label
            >
            <textarea
              id="Message"
              class="bg-[#111827] placeholder:[#9CA2A9] text-gray-100 text-sm rounded-lg block w-full p-2.5"
              placeholder="Let's talk about ... "
              name="Message"
            ></textarea>
          </div>
          <button
            class="z-1 w-[100%!important] px-6 md:px-7 py-3 rounded-full sm:w-max flex justify-center text-white bg-primary border-2 border-transparent"
          >
            Send Message
          </button>
        </form>
      </div>
      <div
        class="bg-gradient-to-tr opacity-25 from-[#570cac] to-primary blur-2xl h-20 w-80 z-0 absolute -top-1/2 -left-4 transform -translate-x-2/3 -translate-1/2"
      ></div>
    </div> -->
  </section>
</template>
<script setup></script>
