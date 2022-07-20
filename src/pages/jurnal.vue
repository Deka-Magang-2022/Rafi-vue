<script setup lang="ts">
import Markdown from '@/assets/jurnal.md';
	useHead({
		title: 'jurnal'
	});

</script>

<template>
	<div>
		<div class="prose border border-black rounded-md p-10">
			<Markdown />

		</div>
	</div>
</template>

<route lang="yaml">
name: 'jurnal'
</route>