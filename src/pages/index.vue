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
				</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">Hobby</h1>
				<div class="text-capitalize text-center  ">
					<p>-Game</p>
					<p>-bulu tangkis</p>
				</div>
			</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">Education</h1>
				<div class="text-capitalize text-center ">
					<p>SD : SDN 005</p>
					<p>SMP : MTS SULAIMAN YASIN</p>
					<p>SMK : TI AIRLANGGA SAMARINDA</p>
				</div>
			</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">skill</h1>
				<div class="text-capitalize text-center ">
				<p>- Laravel Framework PHP</p>
				<p>- css</p>
				<p>- html</p>
				<p>- javascript</p>
				</div>
			</div>
			<div>
				<h1 class="uppercase font-hold text-xl mt-10">About</h1>
				<p class="text-sm text-justify ">Siswa Ti yang Bermotivasi Ingin Mempelajari Programming</p>
			</div>
			<div class="">
				<a href="todo-list">Next</a>

			</div>
		</div>
		</div>
			
		</div>

		<router-link
			:to="{ name: 'other-page' }"
			class="
				mt-5
				text-center
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			"
			>{{ t('pages.other.menu') }}</router-link
		>
	</div>
</template>

<route lang="yaml">
name: home
</route>
