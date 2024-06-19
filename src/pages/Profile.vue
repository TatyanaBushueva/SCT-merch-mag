<script setup></script>

<template>
  <h2 class="text-3xl font-bold mb-8">Профиль</h2>
  <div>
    <label for="user" class="block text-sm font-medium leading-6 text-gray-900">Пользователь</label>
    <div class="relative mt-2 rounded-md shadow-sm">
      <input
        type="text"
        name="user"
        id="user_id"
        class="block w-full rounded-md border-0 py-1.5 pl-7 pr-20 text-gray-900 ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
        placeholder="Например, Иванов Глеб Моисеевич"
      />
    </div>
  </div>
  <div>
    <label for="email" class="block text-sm font-medium leading-6 text-gray-900"
      >Электронная почта</label
    >
    <div class="relative mt-2 rounded-md shadow-sm">
      <input
        type="email"
        name="email"
        id="user_email"
        class="block w-full rounded-md border-0 py-1.5 pl-7 pr-20 text-gray-900 ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
        placeholder="mail@mybox.ru"
      />
    </div>
  </div>
  <div>
    <label for="password" class="block text-sm font-medium leading-6 text-gray-900">Пароль</label>
    <div class="relative mt-2 rounded-md shadow-sm">
      <input
        type="password"
        name="password"
        id="user_pas"
        class="block w-full rounded-md border-0 py-1.5 pl-7 pr-20 text-gray-900 ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
      />
    </div>
  </div>
  <button
    class="mt-4 transition bg-lime-500 w-full rounded-xl py-3 text-white disabled:bg-slate-300 hover:bg-lime-600 active:bg-lime-700 cursor-pointer"
  >
    Добавить
  </button>
</template>
