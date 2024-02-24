<script setup>
definePageMeta({
  layout: "landing",
});
</script>

<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>Contact Us</template>
      <template v-slot:desc>for Sponsorship & Collaboration Event</template>
    </LandingSectionhead>

    <div class="grid md:grid-cols-2 gap-10 mx-auto max-w-4xl mt-16">
      <div>
        <h2 class="font-medium text-2xl text-gray-800">
          Contact Nuxtship Creator
        </h2>
        <p class="text-lg leading-relaxed text-slate-500 mt-3">
          Have a desire to collaborate and sponsor activities? contact us at social media or send
          email.
        </p>
        <div class="mt-5">
          <nuxt-link to="https://maps.app.goo.gl/pTKpvAWDaVvEr9Cc8">
            <div class="flex items-center mt-2 space-x-2 text-gray-600">
              <Icon class="text-gray-400 w-4 h-4" name="uil:map-marker" />
              <span>SEKRETARIAT KAMABA YOGYAKARTA</span>
            </div>
          </nuxt-link>
          <nuxt-link to="https://www.instagram.com/kamaba_yk/">
            <div class="flex items-center mt-2 space-x-2 text-gray-600">
              <Icon class="text-gray-400 w-4 h-4" name="uil:instagram" />
              <span>Kamaba_Yk</span>
            </div>
          </nuxt-link>
          <nuxt-link to="mailto:ilhamkurniawanjateng@gmail.com">
            <div class="flex items-center mt-2 space-x-2 text-gray-600">
              <Icon class="text-gray-400 w-4 h-4" name="uil:envelope" /><a
                >ilhamkurniawanjateng@gmail.com</a>
            </div>
          </nuxt-link>
          <nuxt-link to="https://api.whatsapp.com/send?phone=6282139859517&text=halo%20selamat%20siang%20saya%20tertarik%20dengan%20produk%20website%20bapak.">
            <div class="flex items-center mt-2 space-x-2 text-gray-600">
              <Icon class="text-gray-400 w-4 h-4" name="uil:phone" /><a
                >+62 (877) 3437 8825</a
              >
            </div>
          </nuxt-link>
        </div>
      </div>
      <div>
        <LandingContactform />
      </div>
    </div>
  </LandingContainer>
</template>
