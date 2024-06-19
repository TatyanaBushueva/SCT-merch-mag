<script setup>
/* Шапка (header) */
defineProps({
  totalPrice: Number
})

const emit = defineEmits(['openDrawer'])
</script>

<template>
  <header class="flex justify-between border-b border-slate-200 px-10 py-8">
    <router-link to="/"
      ><div class="flex items-center gap-4">
        <img src="/logo.png" alt="Logo" class="w-14" />
        <div>
          <h2 class="text-xl font-bold uppercase">SCT Merch Mag</h2>
          <p class="text-slate-400">Магазин фирменных мерчей команды Shukhov Cyber Team (SCT)</p>
        </div>
      </div></router-link
    >

    <ul class="flex items-center gap-10">
      <router-link to="/Profile">
        <li class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
          <img src="/profile.svg" alt="Cart" />
          <span>Профиль</span>
        </li>
      </router-link>
      <router-link to="/favorites">
        <li class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
          <img src="/heart.svg" alt="Cart" />
          <span>Избранное</span>
        </li>
      </router-link>
      <li
        @click="() => emit('openDrawer')"
        class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black"
      >
        <img src="/cart.svg" alt="Cart" />
        <b>{{ totalPrice }} руб.</b>
      </li>
    </ul>
  </header>
</template>
