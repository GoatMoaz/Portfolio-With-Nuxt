<template>
  <div class="border-b p-4">
    <h2
      class="text-center text-4xl font-bold mb-4"
      :class="{ 'text-white ': dark, 'text-black': !dark }"
    >
      Get to know me
    </h2>
    <div
      class="flex justify-between items-center mb-16 max-w-4xl mx-auto lg:flex-col"
    >
      <img
        src="/me.jpg"
        alt="Avatar of Moaz Ayman"
        class="rounded-full w-32 h-32 object-cover mb-4"
      />
      <div
        class="flex-1 text-xl ml-6 lg:text-lg lg:text-center lg:ml-0"
        :class="{ 'text-[#cbd5e0] ': dark, 'text-slate-950': !dark }"
      >
        My commitment to learning and applying modern web technologies positions
        me as a promising developer in the tech industry. I'm always eager to
        take on new challenges and continue growing my skills to stay at the
        forefront of web development.
      </div>
    </div>
  </div>
</template>

<script setup>
const { $dark } = useNuxtApp();
const dark = ref($dark);
</script>

<style scoped>
</style>