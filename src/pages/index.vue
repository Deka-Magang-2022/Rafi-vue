<script setup lang="ts">
	import { useStore } from '@/store';
	import VitailseLogo from '@/assets/logo.png';
	useHead({
		title: 'Vitailse | Opinionated vite starter template',
	});

	const store = useStore();
	const { t } = useI18n();
</script>

<template>
	<div class="grid place-items-center min-h-[80vh]">
		<div class="grid bg-emerald-400 border-4 border-red-600 text-stone-900 dark:bg-green-600/40 px-10 py-10 shadow-2x1
		dark:shadow-sky-500 rounded w-full max-w-2xl dark:border-teal-400 text-center place-items-center
		dark:text-yellow-500 ouline outline-dark-900 min-h-[80vh]">
			<div class="grid max-w-2xl text-center rounded-full place-items-center">	
				<img :src="VitailseLogo" width="300" class="mx-auto" />
			
			</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">PROFIL</h1>
				<div class="text-capitalize text-center	 ">
					<p>Nama : M.Rafi Nur Rizki</p>
					<p>Tanggal Lahir : 10-mei-2005</p>
					<p>Agama : islam</p>
					<p>Jenis Kelamin : laki-laki</p>
				</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">contact</h1>
				<div class="text-capitalize text-center	 ">
					<p>No Telepon : 0821-5520-4061</p>
					<p>Email : kaptraf369@gmail.com</p>
					<p><a href="https://github.com/Deka-Magang-2022/Rafi-vue/pulls">* GitHub *</a></p>
				</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">Hobby</h1>
				<div class="text-capitalize text-center  ">
					<p>-Gaming</p>
					<p>-Bulu Tangkis</p>
				</div>
			</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">Education</h1>
				<div class="text-capitalize text-center ">
					<p><a class="text-black-700 dark:text-sky-300 dark:hover:text-sky-200 font-semibold" href="https://www.google.com/maps/place/Gedung+Pertemuan+SDN+005+Samarinda+Ilir/@-0.4934727,117.1621823,20.67z/data=!4m12!1m6!3m5!1s0x2df67fa51beb797f:0x545bae808dedfa6e!2sSMP+NEGERI+6+SAMARINDA!8m2!3d-0.4911339!4d117.1612508!3m4!1s0x2df67f4e0eadf647:0x8f9a35f10941ce04!8m2!3d-0.4934272!4d117.1622486"> * SDN 005</a> </p>
					<p><a class="text-black-700 dark:text-sky-300 dark:hover:text-sky-200 font-semibold" href="https://www.google.com/maps/place/Madrasah+Tsanawiyah+Sulaiman+Yasin/@-0.4909931,117.1571426,17z/data=!3m1!4b1!4m5!3m4!1s0x2df67f6f3984dca3:0xd7a44486b8fde19b!8m2!3d-0.4909985!4d117.1593313"> * MTS SULAIMAN YASIN</a></p>
					<p><a class="text-black-700 dark:text-sky-300 dark:hover:text-sky-200 font-semibold" href="https://www.google.com/maps/place/SMKTI+Airlangga/@-0.4851169,117.1462529,17z/data=!3m1!4b1!4m5!3m4!1s0x2df67f1489bfeb63:0xe1ef6869246e2125!8m2!3d-0.4851223!4d117.1484416">* SMK TI AIRLANGGA</a></p>
				</div>
			</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">skill</h1>
				<div class="text-capitalize text-center ">
				<p>- Laravel Framework PHP</p>
				<p>- html</p>
				<p>- SQL</p>
				<p>- JavaScript</p>
				<p>- CSS (tailwind)</p>
				</div>
			</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">About</h1>
				<p class="text-capitalize text-center ">Siswa Ti yang Bermotivasi Ingin Mempelajari Programming</p>
			</div>

			<div class="max-w-2xl w-full grid grid-flow-row grid-cols-3 gap-5 mt-10 px-4 py-3">
				<a href="todo-list" class="px-4 py-3 bg-red-600 border-double border-4 border-black-500 rounded-md mt-5 text-center text-sm text-justify hover:text-gray-500 dark:hover:text-black hover:underline">Halaman Todo List</a>
				<a href="color-switcher" class="px-4 py-3 bg-red-600 border-double border-4 border-black-500 rounded-md mt-5 text-center text-sm text-justify hover:text-gray-500 dark:hover:text-black hover:underline">Color Swicther</a>
				<a href="kalkulator" class="px-4 py-3 bg-red-600 border-double border-4 border-black-500 rounded-md mt-5 text-center text-sm text-justify hover:text-gray-500 dark:hover:text-black hover:underline">Kalkulator</a>
				<a href="jurnal" class="px-4 py-3 bg-red-600 border-double border-4 border-black-500 rounded-md mt-5 text-center text-sm text-justify hover:text-gray-500 dark:hover:text-black hover:underline">Halaman Jurnal</a>
				<a href="rng" class="px-4 py-3 bg-red-600 border-double border-4 border-black-500 rounded-md mt-5 text-center text-sm text-justify hover:text-gray-500 dark:hover:text-black hover:underline">Halaman RNG</a>
				<!-- <a href="random-number" class="px-4 py-3 bg-red-600 border-double border-4 border-black-500 rounded-md mt-5 text-center text-sm text-justify hover:text-gray-500 dark:hover:text-black hover:underline">Halaman RNG</a> -->
			</div>
			<div class="flexs items-center">...</div>

			
		</div>
		</div>
			
		</div>

	</div>
</template>

<route lang="yaml">
name: home
</route>
