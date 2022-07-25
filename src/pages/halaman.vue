<script setup lang="ts">
	useHead({
		title: 'halaman',
	});
import bg1 from '@/assets/img/bg2.png';
import bg2 from '@/assets/img/bg1.png';
import bg3 from '@/assets/img/bg3.png';
import bg4 from '@/assets/img/bg4.png';
import bg5 from '@/assets/img/bg5.png';
import bg6 from '@/assets/img/bg6.png';
import bg7 from '@/assets/img/bg7.png';
import bg8 from '@/assets/img/bg8.png';
import bg9 from '@/assets/img/bg9.png';
</script>

<template>
	<div>
		
		<div class="grid grid-cols-3 grid-rows-3 min-h-screen grid-flow-col ">
			<div class="col-span-2 row-span-3 bg-[#f2cf77] ">
				<nav class="items-center text-[#005564] bg-[#f2cf77]  ">
					<div class=" font-serif font-bold flex items-center h-full">
						<a href="" class="my-5 mr-72 mx-16 uppercase text-2xl">shave</a>
						<div>
							<a class="mx-2 hover:text-white" href=""> How It Wors </a>
						</div>
						<div>
							<a class="mx-2 hover:text-white" href=""> product </a>
						</div>
						<div>
							<a class="mx-2 hover:text-white" href=""> gifts </a>
						</div>
						<div>
							<a class="mx-2 hover:text-white" href=""> Join Today </a>
						</div>
					</div>
				</nav>
				<div class="bg-[#f2cf77]  min-h-screen ">
					<div class="m-16">
						<p
							class="flex leading-snug tracking-wider text-5xl  font-medium  text-[#005564] font-serif text-left">
							The ultimate app that help you find
							the righ high-quality blade for your face</p>
					</div>
					<div class=" transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110  duration-300 ">
						<a class="hover:bg-[#3aa7aa] py-4 font-semibold  mx-16 uppercase text-xl font-serif text-[#f2cf77] bg-[#005564] px-24"
							href="">get started</a>
					</div>
					<div class="flex justify-end w-auto h-72 px-32">
						<img :src="bg1">
					</div>
				</div>
			</div>
			<div
				class="row-span-1  flex justify-center leading-tight tracking-wider  font-serif text-lg text-white bg-[#d66674]">
				<div class=" mx-24 ">
					<p class=" my-8  text-center  ">
						We have high-quality goomming gift for everyone.
						you'll find gift sets, giftcards, and more!
					</p>
					<div
						class=" transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110 hover:bg-[#3aa7aa] duration-300  p-2 my-8 mb-20 text-[#003851] bg-[#93dbde] ">
						<a href="" class=" flex justify-center  uppercase">shop the gift sets</a>
					</div>
				</div>
			</div>
			<div class="row-span-2 grid grid-cols-3 grid-rows-3  bg-yellow-500 col-span-2">

				<div class=" flex justify-center  bg-red-500 "><img :src="bg1" width=""></div>
				<div class=" flex justify-center  bg-blue-500 "><img :src="bg2" width=""></div>
				<div class=" flex justify-center  bg-green-500 "><img	 :src="bg3" width=""></div>
				<div class=" flex justify-center  bg-gray-500 "><img :src="bg4" width=""></div>
				<div class=" flex justify-center  bg-purple-500 "><img :src="bg5" width=""></div>
				<div class=" flex justify-center  bg-amber-500 "><img :src="bg6" width=""></div>
				<div class=" flex justify-center  bg-cyan-500 "><img :src="bg7" width=""></div>
				<div class=" flex justify-center  bg-blue-500 "><img :src="bg8" width=""></div>
				<div class=" flex justify-center  bg-sky-500 "><img :src="bg9" width=""></div>
			</div>
		</div>
	</div>
	
	<!-- <router-link :to="{ name: 'home' }" class="
				mt-5
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			">{{ $t('pages.home') }}</router-link> -->
</template>

<style scoped></style>

<route lang="yaml">
name: halaman
</route>