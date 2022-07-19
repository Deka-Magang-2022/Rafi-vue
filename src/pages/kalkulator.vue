<script setup lang="ts">
	useHead({
		title: 'Kalkulator',
	});
	import { useStore } from '@/store';
	const store = useStore();
	store.input = ''
	store.temp = ''
	const addNumber = (number) => {
		store.input += number
	}
	const clearData = () => {
		store.input = ''
		store.temp = ''
	}
	const hapus = () => {
		store.input = store.input.slice(0, -1)
	}
	const hitung = (operasi) => {
		if (operasi !== '=') {
			store.input += operasi
		}else{
			try {
				store.temp = eval(store.input.replace(/X/g, '*'))	
			} catch (error) {
				store.temp = 'Error'
			}
			store.input = ''
		}
	}
	const checkInteger = (number) => {
		if (Number.isInteger(number)) {
			return 'bg-green-500 text-white'
		}else{
			return ''
		}
	}
</script>

<template>
	<div>
		<div class="border rounded-md p-5 border-black max-w-lg mb-10">
			<div class="grid gap-5">
				<div class="text-right px-2 py-2" :class="[
					store.temp == 'Error' ? 'bg-red-500 text-white rounded-md' : '',
					checkInteger(store.temp)
				]">
					{{ store.temp }}
				</div>
				<input type="text" class="border border-black rounded-md text-right" disabled v-model="store.input">
			</div>
			<div class="grid grid-cols-4 gap-5 mt-5">
				<div class="grid col-span-4 grid-cols-4 gap-5">
					<button @click="clearData()" type="button" class="col-span-2 bg-gray-100 px-4 py-2 rounded-md border border-black">Clear</button>
					<button @click="hapus()" type="button" class="bg-gray-100 px-4 py-2 rounded-md border border-black">Hapus</button>
					<button @click="hitung('/')" type="button" class="bg-gray-100 px-4 py-2 rounded-md border border-black">/</button>
				</div>
				<div class="grid col-span-3 grid-cols-3 gap-5">
					<button @click="addNumber(number)" v-for="(number) in 9" :key="number" type="button" class="bg-gray-100 px-4 py-2 rounded-md border border-black">
						{{ number }}
					</button>
					<button @click="addNumber(0)" type="button" class="bg-gray-100 px-4 py-2 rounded-md border border-black col-span-3">
						0
					</button>
				</div>
				<div class="grid col-span-1 gap-5">
					<button @click="hitung(item)" v-for="(item) in ['X', '-', '+', '=']" :key="item" type="button" class="bg-gray-100 px-4 py-2 rounded-md border border-black">
						{{ item }}
					</button>
				</div>
			</div>
		</div>
		<router-link
			:to="{ name: 'home' }"
			class="
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			"
			>{{ $t('pages.home') }}</router-link
		>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: kalkulator
</route>