<script setup lang="ts">
import { useStore } from '@/store';
const store = useStore();
let variabelInput = '';
	useHead({
		title: 'todo list',
	});
	store.listTodo = [];
	const simpanData = (value) =>{
		store.listTodo.push(value)
	}
	const hapusData = (value) => {
	store.listTodo.splice( value, 1)
	}
</script>

<template>
	<div>
		<div class="min-h[70vh]">
			<h1 class="text-xl">Halaman Todo List</h1>
			<div class="flex shadow-md  ">
				<input v-model="variabelInput" class="w-full shadow-md dark:shadow-green-500 border dark:border-green-500 dark:bg-[#1f2937] rounded"
					type="text">
				<button @click="simpanData(variabelInput)" type="button"
					class="px-4 py-2 shadow dark:shadow-blue-500 bg-blue-500 rounded-md ml-3 text-white">Add</button>
			</div>
			<div class="grid grid-cols-2 dark:  gap-5 my-10">
				<div class="dark:bg-[#1f2937] shadow-md dark:shadow-blue-500 border dark:border-blue-500 px-4 py-2 rounded-md flex justify-between items-center"
					v-for="(item, index) in store.listTodo" :key="index">
					{{ item }}
					<button class="bg-red-500 shadow-md dark:shadow-red-500 px-4 py-2 rounded-md text-white"
						@click="hapusData(index)" type="button">hapus</button>
				</div>
			</div>
		</div>
		<router-link :to="{ name: 'home' }" class="
				mt-5
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			">{{ $t('pages.home') }}</router-link>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: todo-list
</route>