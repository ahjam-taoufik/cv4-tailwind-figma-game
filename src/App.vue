<script setup>
  import { ref } from 'vue';
import Debugger from './components/debugger.vue';

  const toggle=ref(false)
  
    </script>

<template>
    
       <div class="fixed top-1/2 left-0 h-40 w-36   ">    
              <div class="group flex items-center h-1/4 w-1/4 top-0 hover:w-full transition-all duration-300 bg-pink-700 font-semibold px-1  ">
                <img class="w-7 " src="./assets/Game/instagram.svg" alt="">
                <span class="text-xl text-white font-bold hidden group-hover:block ml-2">Intagram</span>
              </div>

              <div class="group flex items-center h-1/4 w-1/4 top-0 hover:w-full transition-all duration-300 bg-blue-700 font-semibold px-1  ">
                <img class="w-7 " src="./assets/Game/facebook.svg" alt="">
                <span class="text-xl text-white font-bold hidden group-hover:block ml-2">faceook</span>
              </div>
              <div class="group flex items-center h-1/4 w-1/4 top-0 hover:w-full transition-all duration-300 bg-gray-50 font-semibold px-1  ">
                <img class="w-7 " src="./assets/Game/youtube.svg" alt="">
                <span class="text-xl text-gray-500 font-bold hidden group-hover:block ml-2">Youtube</span>
              </div>
              <div class="group flex items-center h-1/4 w-1/4 top-0 hover:w-full transition-all duration-300 bg-blue-800 font-semibold px-1  ">
                <img class="w-7 " src="./assets/Game/linkedin.svg" alt="">
                <span class="text-xl text-white font-bold hidden group-hover:block ml-2">LinkedIn</span>
              </div>
              <div class="group flex items-center h-1/4 w-1/4 top-0 hover:w-full transition-all duration-300 bg-blue-600 font-semibold px-1  ">
                <img class="w-7 " src="./assets/Game/twitter.svg" alt="">
                <span class="text-xl text-white font-bold hidden group-hover:block ml-2">Twitter</span>
              </div>
       </div>

        <div class="relative bg-primary-color h-screen pt-6">

            <!--start drawer -->
            <div
            @click="toggle=!toggle"
            :class="[toggle ? 'block' : 'hidden']"
             class="bg-red-200 opacity-60 inset-0 absolute z-10 lg:hidden ">
            </div>


            <div class="lg:hidden  inline-block absolute right-0 z-20">
              <img @click="toggle=!toggle" class=" h-8 ml-auto mr-4 cursor-pointer"  src="./assets/Game/menu.svg" alt="">
            </div>


            <div 
            :class="[toggle ? 'left-0' : '-left-full']"
            class="absolute text-white  top-0 transition-all ease-in-out duration-700 h-full w-3/4 z-10 bg-black/95  lg:hidden">
                 drawer
              </div>
            <!--end drawer -->





            <div class="relative flex flex-col justify-between  h-full  w-10/12 mx-20 ">
              
                <nav class="text-white hidden lg:flex lg:justify-between lg:items-center">
                  <div class="font-extrabold text-3xl">LG.</div>
                  <div class="space-x-40 font-bold ">
                    <a href="#"><span>About</span></a>
                    <a href="#"><span>Service</span></a>
                    <a href="#"><span>Our Work</span></a>
                  </div>
                </nav>
              

                <div class=" h-5/6 flex justify-between items-end">
                
                  <div class=" self-center space-y-20">
                    <h1  class=" text-6xl m-0 p-0 border-none shadow font-extrabold tracking-wide">Learn The art of  Game Dev</h1>
                    <p class="text-xl shadow font-semibold">This is a comprehensive course on Game Development. <br>
                      You will learn everything from generating an idea to <br>
                      publishing your games to different platforms.
                    </p>

                    <button class="shadow-2xl text-white font-semibold text-xl bg-orange-500  py-4 px-10 hover:bg-orange-300 rounded-full">
                      <span>Endoll Now</span>
                    </button>

                  </div>

                  <div class="">
                    <img class="h-[700px]" src="./assets/Game/hero-image.png" alt="">
                  </div>
                </div>

                <span class="hidden lg:block absolute text-xl font-extrabold shadow-2xl text-center left-1/2 top-1/2 p-4 rounded-2xl bg-gray-400 ">
                  37K <br>
                  Student Enrolled
                </span>

                <span class="hidden lg:block absolute text-xl font-extrabold shadow-2xl text-center left-[40%] top-2/3 p-4 rounded-2xl bg-gray-400 ">
                  3.7K <br>
                  Overall Rating
                </span>
            </div>
        </div>
        <!-- <div class="inline-block bg-gray-300 h-20">
        </div> -->

    
      <Debugger/>
  </template>



<style>
  .shadow {
    /* text-shadow: -1px 7px 5px rgba(6,15,39,0.78); */
    border: none;
    
  }
</style>
