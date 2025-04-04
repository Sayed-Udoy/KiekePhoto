<script setup lang="ts">
import i1 from "../../assets/Home/Levensverhalen/i1.png";
import i2 from "../../assets/Home/Levensverhalen/i2.png";
import i3 from "../../assets/Home/Levensverhalen/i3.png";
</script>

<template>
  <section class="bg-[#F9F5F466] py-10">
    <div class="container px-2 md:flex gap-10">
      <!-- left side  -->
      <div>
        <div class="py-5">
          <h1
            class="text-[40px] md:text-[48px] lg:text-[54px] font-newYork uppercase leading-[120%]"
          >
            Levensver <span class="text-[#2D3B3BE5]">halen</span>
          </h1>
          <p
            class="text-[14px] md:text-[16px] lg:text-[20px] text-[#2D3B3BE5] py-4"
          >
            Dive into the world of photography through insightful articles,
            expert tips, and creative inspiration.
          </p>
        </div>
        <div class="md:flex gap-4">
          <div class="flex-1">
            <img :src="i1" alt="" />
            <div class="pt-3 pb-4">
              <h1
                class="text-[#2D3B3BE5] text-[18px] font-[500] md:text-[24px] leading-[140%] capitalize pt-3"
              >
                The Art of Minimalist Photography: Less is More
              </h1>
              <p
                class="text-[#2D3B3BE5] text-[14px] md:text-[18px] leading-[150%] capitalize py-2"
              >
                Discover how simplicity can enhance storytelling in photography.
                This blog explores the power of negative space, clean
                compositions, and subtle elegance in creating timeless images.
              </p>
            </div>
          </div>
          <div class="hidden flex-1 w-[100%] md:flex flex-col-reverse">
            <img
              class="max-h-[350px] bg-cover object-fit-content"
              :src="i2"
              alt=""
            />
            <div>
              <h1
                class="text-[#2D3B3BE5] font-[500] text-[18px] md:text-[24px] leading-[140%] capitalize pt-3"
              >
                The Art of Minimalist Photography: Less is More
              </h1>
              <p
                class="text-[#2D3B3BE5] text-[14px] md:text-[18px] leading-[150%] capitalize py-2"
              >
                Discover how simplicity can enhance storytelling in photography.
                This blog explores the power of negative space, clean
                compositions, and subtle elegance in creating timeless images.
              </p>
            </div>
          </div>
        </div>
      </div>
      <!-- right side  -->
      <div>
        <div class="hidden md:flex flex-col">
          <img :src="i3" alt="" />
          <div>
            <h1
              class="text-[#2D3B3BE5] font-[500] text-[18px] md:text-[24px] leading-[140%] capitalize pt-3"
            >
              The Art of Minimalist Photography: Less is More
            </h1>
            <p
              class="text-[#2D3B3BE5] mb-3 text-[14px] md:text-[18px] leading-[150%] capitalize py-2"
            >
              Discover how simplicity can enhance storytelling in photography.
              This blog explores the power of negative space, clean
              compositions, and subtle elegance in creating timeless images.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
