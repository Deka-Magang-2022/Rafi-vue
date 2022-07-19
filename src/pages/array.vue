<script setup lang="ts">
	useHead({
		title: 'Other Pages',
	});
const chars = [1,1,2,2,2,3,4,4,5,5,5];
const uniqueChars = [...new Set(chars)];

console.log(uniqueChars);

</script>

<template>
    <div>
        <div>
            {{ uniqueChars }}
        </div>
        <router-link :to="{ name: 'home' }" 
			class="
				mt-5
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			
			">{{ $t('pages.home') }}</router-link>
		>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: other-page
</route>



</template>
