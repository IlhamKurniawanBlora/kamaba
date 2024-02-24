<script setup>
const tahun = new Date().getFullYear();
const TeamImg1 = "https://source.unsplash.com/IF9TK5Uy-KI";
const TeamImg2 = "https://source.unsplash.com/iEEBWgY_6lA";
const TeamImg3 = "https://source.unsplash.com/ZHvM3XIOHoE";
const icons = [
{
    icon: "bx:bxs-bulb",
  }
]
const team = [
  {
    name: "Anik Ida",
    title: "Wakil Ketua",
    avatar: {
      src: TeamImg1,
      width: 480,
      height: 560,
    },
  },
  {
    name: "Khoirul Anam",
    title: "Ketua Umum",
    avatar: {
      src: TeamImg2,
      width: 580,
      height: 580,
    },
  },
  {
    name: "Faza Azzahro",
    title: "Bendahara",
    avatar: {
      src: TeamImg3,
      width: 580,
      height: 580,
    },
  },
];
</script>
<template>
  <div class="bg-black px-20 py-20 mt-20 mx-auto max-w-5xl rounded-lg flex flex-col items-center text-center">
    <h2 class="text-white text-3xl md:text-6xl">organizational structure</h2>
    <p class="text-slate-500 mt-4 text-lg md:text-xl">
      kamaba administrator of the year <span>{{ tahun }}</span>
    </p>
    <div class="grid md:grid-cols-3 gap-10 mx-auto max-w-4xl mt-12">
      <div v-for="item of team" class="group">
        <div class="w-full aspect-square">
          <img
            :src="item.avatar.src"
            :width="item.avatar.width"
            :height="item.avatar.height"
            format="avif"
            alt="Team"
            class="w-full h-full object-cover rounded-full transition group-hover:-translate-y-1 group-hover:shadow-xl"
          />
        </div>

        <div class="mt-4 text-center">
          <h2 class="text-lg text-gray-800">{{ item.name }}</h2>
          <h3 class="text-sm text-slate-500">{{ item.title }}</h3>
        </div>
      </div>
    </div>
    <div class="flex mt-5">
      <LandingLink href="#" styleName="outline" class="hover:border-white">Show More
      </LandingLink>
    </div>
  </div>
</template>
