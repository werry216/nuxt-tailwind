<template>
  <div class="bg-gray-100 font-sans w-full min-h-screen m-0">
    <Header></Header>
    <div class="w-full rounded-lg sahdow-lg p-12 flex flex-col justify-center items-center">
        <div class="text-center">
            <p class="mb-3 text-6xl">Deine Job website</p>
        </div>
        <div class="mb-8">
            <img class="object-center object-cover rounded-full h-418 w-405" src="/images/undraw_agreement_aajr.png" alt="Undraw agreement">
        </div>
    </div>
    <div class="bg-white shadow border-t-4 h-32 rounded-t-lg">
        <div class="container mx-auto px-4">
            <div class="block sm:hidden bg-white py-2">
                <div class="flex flex-col">
                    <div class="flex items-center pt-2 bg-gradient-to-r from-green-400 to-blue-500 rounded-full py-3 px-6 justify-center text-sm font-semibold text-white">
                        Kostenlos Registrieren
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import Header from "~/components/Header";
export default {
  components: {
    Header,
  }
}
</script>
