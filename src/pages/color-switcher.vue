<script setup lang="ts">
useHead({
  title: "color-switcher",
});
import { useStore } from '@/store';
const store = useStore();
store.color = 'bg-red-500'
store.text  = 'text-white'
</script>

<template>
  <div class="grid gap-10">
		<div class="flex flex-col w-full gap-10">
			<div :class="store.color" class="w-full p-10 rounded-md">
				<p :class="store.text" class="text-xl text-blue-500 font-semibold">Sebuah Text</p>
			</div>
			<div class="grid grid-cols-4 gap-5">
				<button type="button" @click="store.color = 'bg-blue-500'" class="bg-blue-500 hover:bg-blue-600 text-white px-4 py-2 rounded-md">Ganti Bg</button>
				<button type="button" @click="store.color = 'bg-red-500'" class="bg-red-500 hover:bg-red-600 text-white px-4 py-2 rounded-md">Ganti Bg</button>
				<button type="button" @click="store.color = 'bg-green-500'" class="bg-green-500 hover:bg-green-600 text-white px-4 py-2 rounded-md">Ganti Bg</button>
				<button type="button" @click="store.color = 'bg-black'" class="bg-black hover:bg-black/80 text-white px-4 py-2 rounded-md">Ganti Bg</button>
			</div>

            <div class="grid grid-cols-4 gap-5">
                <button type="button" @click="store.text = 'text-blue-500'" class="bg-blue-500 hover:text-green-600 text-blue px-4 py-2 rounded-md">Ganti text</button>
				<button type="button" @click="store.text = 'text-red-500'" class="bg-red-500 hover:bg-red-600 text-white px-4 py-2 rounded-md">Ganti text</button>
				<button type="button" @click="store.text = 'text-green-500'" class="bg-green-500 hover:bg-green-600 text-white px-4 py-2 rounded-md">Ganti text</button>
				<button type="button" @click="store.text = 'text-black'" class="bg-black hover:bg-black/80 text-white px-4 py-2 rounded-md">Ganti text</button>
            </div>
		</div>

        
    <router-link
      :to="{ name: 'home' }"
      class="mt-5 hover:text-gray-200 dark:hover:text-gray-500 hover:underline"
      >{{ $t("pages.home") }}</router-link
    >
  </div>
</template>

<style scoped></style>

<route lang="yaml">
name: color-switcher
</route>
