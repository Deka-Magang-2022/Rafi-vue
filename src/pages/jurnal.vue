<script setup lang="ts">

import Bulan1 from '@/assets/bulan1.md';

useHead({
    title: 'jurnal',
});

// const rafiAngka = [1,1,2,2,2,3,4,4,5,5,5];
// const arrayAngka = [...new Set(rafiAngka)];

// console.log(arrayAngka);

</script>

<template>
    <div>
    
    <div class="my-10 prose border border-black rounded-md p-10">
        <Bulan1 />
    </div>
    <router-link
			:to="{ name: 'home' }"
			class="
				mt-5
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			"
			>{{ $t('pages.home') }}</router-link
		>
	</div>
</template>

<style scoped>
</style>

<route lang="yaml">
name: jurnal
</route>