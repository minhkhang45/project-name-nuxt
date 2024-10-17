<template>
  <div class="header flex justify-center">
    <div class="max-w-[926px]">
      <h2 class="text-white font-bold text-6xl">Enter a world of <span class="text-[#00bdfe]">Photos</span> & Amazing
        <span class="text-[#00bdfe]">Awards</span>
      </h2>
      <p class="text-white py-[30px] mt-[40px] mx-[75px] border-t border-slate-500/50">SnapX Photography is a
        professional website template with 5 different HTML pages for maximum customizations. It is free for commercial
        usage. This Bootstrap v5.1.3 CSS layout is provided by TemplateMo Free CSS Templates.</p>
      <div class="flex justify-center">
        <button
          class="transition duration-300 border-[#ffffff] border hover:bg-[#ffffff] hover:text-[#00bdfe] rounded-[10px] px-[30px] py-[15px] my-auto h-fit text-[#ffffff] flex items-center font-medium text-xl mr-[15px]">
          Explore SnapX Contest
        </button>
        <button
          class="transition duration-300 border-0 hover:text-[#00bdfe] p-[10px] text-white font-medium flex items-center">
          <Icon name="fluent:play-12-filled" class="text-xl mr-2" />Watch Our Video Now
        </button>
      </div>
    </div>
  </div>
  <div class="mt-[-150px] relative">
    <Swiper class="max-w-7xl !static" :key="1" :modules="[SwiperAutoplay, SwiperNavigation]" :slides-per-view="3"
      :space-between="20" navigation :loop="true" :autoplay="{
        delay: 4000,
        disableOnInteraction: true,
      }">
      <SwiperSlide v-for="(slide, idx) in slides" :key="idx" class="swipe">
        <img class="w-full rounded-[15px] swiper-img" :src="slide.url" alt="">
        <div class="bg-white rounded-[15px] hov flex flex-col justify-center items-center ">
          <p class="text-center text-2xl text-[#00bdfe] mb-[22px]">{{ slide.title }} <Icon name="ph:star-fill"
              v-for="i in slide.stars" class="text-lg"></Icon>
          </p>
          <ul class="space-y-2">
            <li class="text-sm text-center">
              <span class="  ">Contest Winner:</span>
              <span class="text-[#afafaf]"> Thomas Eddy</span>
            </li>
            <li class="text-sm text-center">
              <span class="  ">Contest Author:</span>
              <span class="text-[#afafaf]"> Antony Soft</span>
            </li>
            <li class="text-sm text-center">
              <span class="  ">Awards:</span>
              <span class="text-[#afafaf]"> 100$</span>
            </li>
          </ul>
        </div>
      </SwiperSlide>
    </Swiper>
  </div>
  <div class="mt-[120px] px-[65px] ">
    <div class="flex justify-between">
      <div>
        <p class="text-[#00bdfe]">Our Categories</p>
        <h4 class="text-3xl font-bold">Check Out <span class="text-[#00bdfe]">Popular</span> Contest <span
            class="text-[#00bdfe]">Categories</span> </h4>
      </div>
      <div>
        <button
          class="border rounded-xl border-[#00bdfe] bg-[#00bdfe] px-[30px] py-[10px] text-white font-medium">Discover All
          Categories</button>
      </div>
    </div>
    <div class="flex justify-center">
      <div v-for="i in cyegor" class="border rounded-[15px] w-full mx-[12px] p-[30px]">
        <div class="flex">
          <div class="bg-[#f7f7f7] rounded-[10px] flex items-center justify-center w-[75px] h-[75px] mr-[20px]">
            <img :src="i.icon" alt="">
          </div>
          <div>
            <p class="font-bold text-xl">{{ i.title }} Pic Contest</p>
            <p><span class="rounded-tl-[10px] rounded-br-[10px] px-[9px] py-[5px] shadow1 font-medium text-[#00bdfe]">{{ i.avaible }}</span><span class="text-[#afafaf]"> Available Contests</span></p>
          </div>
        </div>
        <div>
          
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
const slides = [
  {
    url: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/featured-01.jpg",
    title: "Walk In The Nature",
    stars: 3
  },
  {
    url: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/featured-02.jpg",
    title: "Happy In The Nature",
    stars: 4
  },
  {
    url: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/featured-03.jpg",
    title: "Run In The Nature ",
    stars: 1
  },
  {
    url: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/featured-01.jpg",
    title: "Walk In The Nature",
    stars: 3
  },
  {
    url: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/featured-02.jpg",
    title: "Happy In The Nature",
    stars: 4
  },
  {
    url: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/featured-03.jpg",
    title: "Run In The Nature ",
    stars: 1
  }
]
const cyegor = [
  {
    icon: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/icon-01.png",
    avaible: 126,
    picture: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/popular-01.png",
    title: "Nature"
  },
  {
    icon: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/icon-02.png",
    avaible: 116,
    picture: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/popular-02.png",
    title: "Random"
  },
  {
    icon: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/icon-03.png",
    avaible: 164,
    picture: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/popular-03.png",
    title: "Portrait"
  },
  {
    icon: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/icon-04.png",
    avaible: 135,
    picture: "https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/popular-04.png",
    title: "Space"
  },
]
</script>

<style>
.shadow1 {
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.06);
}
.header {
  background-image: url(/public/banner-bg.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  padding-top: 290px;
  padding-bottom: 240px;
  text-align: center;
  background-color: #2a2a2a;
}

.swiper-slide {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 18px;
  height: 300px;
  width: 412px !important;
  font-size: 4rem;
  font-weight: bold;
  font-family: 'Roboto', sans-serif;
  position: relative;
}

.swiper-wrapper {
  width: 100px;
}

.swiper-cards {
  width: 412px;
  height: 300px;
}

.swiper-cards .swiper-slide {
  border-radius: 6px;
  border: 1px solid black;
}

.swiper-button-next,
.swiper-button-prev {
  min-width: 50px;
  min-height: 50px;
  border-radius: 50%;
  background: #00bdfe;
  opacity: 0.75;
  color: #fff;
  transition: all .3s;
}

.swiper-button-next {
  right: 200px;
}

.swiper-button-prev {
  left: 200px;
}

.swiper-button-next:hover,
.swiper-button-prev:hover {
  opacity: 1;
  background: #00bdfe;
}

.swiper-button-prev::after,
.swiper-button-next::after {
  font-size: 20px;
  font-weight: 900;
}

.swiper-slide .hov {
  position: absolute;
  bottom: -100%;
  width: 100%;
  height: 100%;
  transition: all .3s;
  opacity: 0;
}

.swiper-slide:hover .hov {
  bottom: 0;
  opacity: 0.92;
}
</style>