
<template>
<div class="bg-[#111827] min-h-screen">
  <NavBar />
  <HeroSection />
  <ServiceSection/>
  <AboutSection/>
  <ExperienceSection/>
  <ProjectSection/>
  <ContactSection/>
  <FooterSection/>
  <BackToTop/>
</div>
</template>

<script setup>
import { defineAsyncComponent } from 'vue';
//Import Component Asynchronously
const NavBar = defineAsyncComponent(()=>import('@/components/Navbar.vue'));
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'));
const ServiceSection = defineAsyncComponent(()=>import('@/components/ServiceSection.vue'));
const AboutSection = defineAsyncComponent(()=>import('@/components/AboutSection.vue'));
const ExperienceSection = defineAsyncComponent(()=>import('@/components/ExperienceSection.vue'));
const ProjectSection = defineAsyncComponent(()=>import('@/components/ProjectSection.vue'));
const ContactSection = defineAsyncComponent(()=>import('@/components/ContactSection.vue'));
const FooterSection = defineAsyncComponent(()=>import('@/components/FooterSection.vue'));
const BackToTop = defineAsyncComponent(()=>import('@/components/BackToTop.vue'));
</script>


