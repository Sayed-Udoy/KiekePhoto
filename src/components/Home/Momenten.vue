<script setup lang="ts">
import img1 from "../../assets/Home/moment/img1.png";
import img2 from "../../assets/Home/moment/img2.png";
import img3 from "../../assets/Home/moment/img3.png";
import Love from "../../assets/icons/love.svg";
import Comment from "../../assets/icons/comment.svg";
import Plain from "../../assets/icons/plane.svg";
import Share from "../../assets/icons/share.svg";
import { cardItems } from "../../data/data.ts";
import { cardItems2 } from "../../data/data.ts";
</script>

<template>
  <section class="py-10">
    <div
      class="container h-full px-2 gap-5 place-items-center md:flex overflow-hidden md:max-h-[800px]"
    >
      <!-- left side  -->
      <div class="flex-1">
        <div class="py-2">
          <h1
            class="text-[40px] md:text-[46px] lg:text-[54px] leading-[120%] font-newYork"
          >
            Bijzondere <span class="text-[#2D3B3BB2]">Momenten</span>
          </h1>
          <p class="text-[14px] lg:text-[20px] text-[#2D3B3BE5] mt-2">
            A curated collection of breathtaking visuals that capture moments,
            emotions, and stories.
          </p>
        </div>
        <div class="flex w-full gap-8 md:gap-5 mt-5">
          <div class="flex flex-col gap-6 md:gap-8">
            <img class="w-[100%]" :src="img1" alt="" />
            <img class="w-[100%]" :src="img2" alt="" />
          </div>
          <div>
            <img class="w-[100%]" :src="img3" alt="" />
          </div>
        </div>
      </div>
      <!-- right side  -->
      <div
        class="flex-1 bg-[#F9F5F4] md:px-4 flex flex-col place-items-center mt-10 md:mt-0 md:flex-row md:max-h-[800px]"
      >
        <!-- card 1  -->
        <div
          class="grid grid-cols-3 md:flex md:flex-col overflow-x-scroll min-w-[800px] md:min-w-auto"
        >
          <div
            v-for="(item, index) in cardItems"
            class="max-w-[300px] lg:max-w-[350px] min-w-[250px] py-2 px-2"
          >
            <!-- images  -->
            <div>
              <img
                class="w-full min-h-[250px] md:min-w-auto"
                :src="item.image"
                alt=""
              />
            </div>
            <!-- icons  -->
            <div class="flex justify-between py-2 items-center">
              <div class="flex items-center gap-3">
                <img :src="Love" height="20" width="20" alt="" />
                <img :src="Comment" height="20" width="20" alt="" />
                <img :src="Plain" height="20" width="20" alt="" />
              </div>
              <div>
                <img :src="Share" height="20" width="20" alt="" />
              </div>
            </div>
            <!-- views  -->
            <div>
              <p class="text-[10px]">{{ item.views }} views</p>
              <p class="mt-3 text-[9.32px] md:text-[11.67px] leading-[140%]">
                {{ item.text }}
              </p>
            </div>
          </div>
        </div>
        <!-- card 2  -->
        <div
          class="grid grid-cols-2 md:flex md:flex-col overflow-x-scroll min-w-[600px] md:min-w-auto"
        >
          <div
            v-for="(item, index) in cardItems2"
            :key="index"
            class="max-w-[270px] lg:max-w-[350px] min-w-[250px] md:min-w-auto py-2 px-2"
          >
            <!-- images  -->
            <div>
              <img class="w-full max-h-[250px]" :src="item.image" alt="" />
            </div>
            <!-- icons  -->
            <div class="flex justify-between py-2 items-center">
              <div class="flex items-center gap-3">
                <img :src="Love" height="20" width="20" alt="" />
                <img :src="Comment" height="20" width="20" alt="" />
                <img :src="Plain" height="20" width="20" alt="" />
              </div>
              <div>
                <img :src="Share" height="20" width="20" alt="" />
              </div>
            </div>
            <!-- views  -->
            <div>
              <p class="text-[10px]">{{ item.views }} views</p>
              <p class="mt-3 text-[9.32px] md:text-[11.67px] leading-[140%]">
                {{ item.text }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
