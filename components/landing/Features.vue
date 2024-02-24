<script setup>
const features = [
  {
    title: "Perwakilan Mahasiswa",
    description:
      "Menjadi suara dan perwakilan mahasiswa di berbagai forum, baik di tingkat kampus, regional, atau nasional. Organisasi mahasiswa bertugas untuk menyampaikan aspirasi, kebutuhan, dan pandangan mahasiswa kepada pihak-pihak terkait.",
    icon: "bx:bxs-bulb",
  },
  {
    title: "Pengembangan Soft Skills",
    description:
      "Memberikan platform bagi mahasiswa untuk mengembangkan keterampilan interpersonal, kepemimpinan, dan kemampuan berkomunikasi. Melalui kegiatan organisasi, mahasiswa dapat memperoleh pengalaman praktis yang berharga di luar lingkup akademis.",
    icon: "bx:bxs-happy",
  },
  {
    title: "Pelayanan Sosial dan Kemanusiaan",
    description:
      "Melakukan kegiatan amal, pengabdian masyarakat, dan proyek kemanusiaan. Organisasi mahasiswa dapat menjadi agen perubahan positif dengan memberikan kontribusi pada masyarakat, membantu yang membutuhkan, dan menciptakan dampak positif di lingkungan sekitar.",
    icon: "bx:bxs-donate-heart",
  },
  {
    title: "Pengelolaan Konflik dan Mediasi",
    description:
      "Organisasi mahasiswa dapat berperan dalam menciptakan lingkungan yang harmonis di antara mahasiswa dan dalam menangani konflik yang mungkin timbul di antara anggotanya. Dengan melibatkan mahasiswa dalam kegiatan mediasi, organisasi dapat membantu membangun hubungan yang sehat dan saling mendukung di antara anggotanya.",
    icon: "bx:bxs-home-heart",
  },
  {
    title: "Pengembangan Minat dan Bakat",
    description:
      "Memberikan wadah bagi mahasiswa untuk mengembangkan minat dan bakat di luar akademis. Organisasi mahasiswa seringkali menyelenggarakan kegiatan seni, olahraga, dan budaya yang memungkinkan mahasiswa mengeksplorasi dan mengasah kreativitas serta bakat mereka.",
    icon: "bx:bxs-book-open",
  },
  {
    title: "Pengembangan Komunitas Kehidupan Masyarakat",
    description:
      "Organisasi mahasiswa dapat berperan dalam meningkatkan kesadaran dan keterlibatan mahasiswa dalam kehidupan masyarakat sekitar. Melalui berbagai kegiatan sosial, edukasi, dan proyek pembangunan masyarakat, organisasi tersebut dapat memberikan kontribusi positif dalam meningkatkan kualitas hidup masyarakat sekitar kampus.",
    icon: "bx:bxs-user",
  },
];
</script>

<template>
  <div class="mt-16 md:mt-0">
    <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight">
      What do we do?
    </h2>
    <p class="text-lg mt-4 text-slate-600">
      As a regional student organization, we have several activities to develop ourselves
    </p>
  </div>

  <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
    <div v-for="item of features" class="flex gap-4 items-start">
      <div class="mt-1 bg-black rounded-full p-2 w-8 h-8 shrink-0">
        <Icon class="text-white" :name="item.icon" />
      </div>
      <div>
        <h3 class="font-semibold text-lg">{{ item.title }}</h3>
        <p class="text-slate-500 mt-2 leading-relaxed">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
