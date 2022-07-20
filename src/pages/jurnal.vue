<script setup lang="ts">
import Markdown from "@/assets/jurnal.md";
	useHead({
		title: 'jurnal'
	});

</script>

<template>
	<div>

		<div class="prose border border-black rounded-md p-10">
			<Markdown />
		</div>

			<router-link
			:to="{ name: 'home' }"
			class="
				hover:text-gray-500
				dark:hover:text-gray-200
				hover:underline
			"
			>{{ $t('pages.home') }}</router-link
		>

	</div>
</template>

<route lang="yaml">
name: jurnal
</route>