<template>
    <section class="text-white mt-20" id="project">
        <div class="px-4 xl:pl-16">
            <div class="mb-4 md:flex md:justify-between xl:pr-16">
                <h2 class="text-4xl font-bold text-white">My Project</h2>
                <div class="flex space-x-4 mb-4 mt-5 md:nt-0">
                    <button class="hover:text-pri"
                    v-for="category in ['all','Web development', 'Mobile App','Desktop App']"
                    :key="category"
                    @click="() => selectedCategory = category"
                    >
                  {{category }}
                    </button>
                </div>
            </div>

      <ul class="px-4 sm:py-16 xl:pr-16 grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:gap-10 md:pt-12 lg:grid-cols-3"
                data-aos="fade-right">
                <div v-for="project in filteredProjects" :key="project.id">
                    <div class="h-52 md:h-[24rem] rounded-t-xl relative group"
                    :style="{ backgroundImage: 'url(' + project.image + ')', backgroundSize: 'cover' }">                    
                    <div class="overlay items-center justify-center absolute top-0 left-0 w-full h-full bg-[#181818] bg-opacity-0
                    hidden group-hover:flex group-hover:bg-opacity-80 transition-all duration-500
                    ">
                        <a class="h-14 w-14 mr-2 border-2 relative rounded-full border-[#ADB7BE] hover:border-white group/link"
                            :href="project.webUrl"> <svg xmlns="http://www.w3.org/2000/svg" fill="none"
                                viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true"
                                data-slot="icon"
                                class="h-10 w-10 text-[#ADB7BE] absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2  cursor-pointer group-hover/link:text-white">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M17.25 6.75 22.5 12l-5.25 5.25m-10.5 0L1.5 12l5.25-5.25m7.5-3-4.5 16.5">
                                </path>
                            </svg></a>
                            
                    </div>
                    
                </div>
                
                <div class="text-white rounded-b-xl mt-3 bg-[#111a3e] shadow-lg border border-[#1f1641] py-6 px-4">
                    <h3 class="text-lg font-semibold uppercase lg:text-xl"> {{ project.title }}</h3>
                    <p class="text-[#ADB7BE]">{{ project.description }}</p>
                    
                    <div class="flex flex-wrap p-2.5">
                        <div v-for="technology in project.technologies" :key="technology" class="text-center ml-1 mt-1 rounded-3xl bg-[#111827]"
                        style="box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1); border: 1px solid #111827;backdrop-filter: blur(9px);-webkit-backdrop-filter: blur(9px);"
                        >
                    <p class="px-1 py-2">{{ technology }}</p>
                 
                    </div>
                    </div>
                </div>
                </div>
            </ul>
        </div>
    </section>
  
</template>

<script setup>
import {ref, computed} from 'vue';
const Projects = ref([

    {
        id:1,
        category:'web development',
        image: 'src/assets/pos.png',
        title:'Personal Project',
        description:'Point of Sale (POS) and Inventory Management system designed specifically for gold stores.',
        technologies: ['Laravel','Mysql','JS','Mysql','Bootstrap'],
        webUrl:' https://github.com/LadjamatliAbusood/jewellery'

    },
    {
        id:2,
        category:'Mobile App',
        image: 'src/assets/lan.png',
        title:'Capstone',
        description:'A Food Quality Image Classification for Vegetables using Android Mobile Application',
        technologies: ['Java','ML (Teachable Machine)','HTML','Bootstrap'],
        webUrl:'https://github.com/LadjamatliAbusood/Lanchanika'

    },
    {
        id:3,
        category:'Mobile App',
        image: 'src/assets/and.png',
        title:'Capstone',
        description:'A Mobile Assistive Application of Philippine Currency Recognition For The Visually Impaired',
        technologies: ['JAVA','ML (Teachable Machine)','Python'],
        webUrl:'https://github.com/LadjamatliAbusood/Image_Classification_tflite_Phisos'

    },
    {
        id:4,
        category:'web development',
        image: 'src/assets/cake.png',
        title:'Software Engineering',
        description:'Koffi Sugar Heist Cake Booking System',
        technologies: ['Jave','PHP','Mysql','Itexmo'],
        webUrl:'https://github.com/LadjamatliAbusood/kofissugarheist'

    },
   
    {
        id:5,
        category:'Desktop App',
        image: 'src/assets/desktop.png',
        title:'Personal Project',
        description:'Desktop Application POS  with Networking',
        technologies: ['JAVA','Mysql'],
        webUrl:'https://github.com/LadjamatliAbusood/Point-of-Sale-desktop-app'

    },
 
]);

const selectedCategory=ref('all');
const filteredProjects = computed(()=>{
    if(selectedCategory.value == 'all'){
        return Projects.value;
    }
    return Projects.value.filter(project => project.category.toLocaleLowerCase() === selectedCategory.value.toLocaleLowerCase());
    
});
</script>

