<template>
  <main class="grid lg:grid-cols-2 place-items-center pt-16 pb-8 md:pt-8">
    <div class="p-24 md:order-1 hidden md:block">
      <img
        class=" transition-transform transform hover:scale-125"
        src="~/assets/img/Kamaba.png"
        alt="Starship starts the engine"
        loading="eager"
        format="avif"
        width="502"
        height="502"
      />
    </div>

    <div>
      <h1 class="text-5xl lg:text-6xl xl:text-7xl font-bold lg:tracking-tight">
        Keluarga Mahasiswa Blora Yogyakarta
      </h1>
      <p class="text-lg mt-4 text-slate-600 max-w-xl">
        Kamaba Yogyakarta adalah organisasi mahasiswa yang berasal dari Blora dan berfokus pada mahasiswa yang tengah menempuh pendidikan tinggi di Yogyakarta. Mereka memiliki tujuan untuk merangkul dan menggandeng semua masyarakat Blora yang sedang kuliah atau bekerja di Yogyakarta.<span class="font-semibold ml-2">"Suro Diro Joyoningrat, Lebur Dening Pangastuti"</span>
      </p>
      <div class="mt-6 flex flex-col sm:flex-row gap-3">
        <LandingLink
          href="https://www.instagram.com/kamaba_yk/"
          target="_blank"
          rel="noopener"
           class="hover:text-black hover:bg-white hover:border-black">Visit Us</LandingLink
        >
        <LandingLink
          size="lg"
          styleName="outline"
          rel="noopener"
          href="https://www.instagram.com/kamaba_yk/"
          target="_blank" 
          >Contact Us</LandingLink
        >
      </div>
    </div>
  </main>
</template>
