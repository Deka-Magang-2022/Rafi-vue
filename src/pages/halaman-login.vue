<script setup lang="ts">
	useHead({
		title: 'halaman login',
	});
	
</script>

<template>
	<div>

        <div class="grid place-items-center min-h-[80vh] rounded w-full max-w-2xl border-4 border-gray-600 rounded-md bg-sky-300 flex text-gray-800 antialiased px-4 py-6 flex flex-col flex flex-items-end sm:py-12">
            <div class="relatif py-3 sm:max-w-xl mx-auto text-center">
                        <span class="text-2xl font-bold text-blue-500 flex justify-center">Login to FaceBook</span>
                <div class="relative mt-4 bg-white shadow-md sm:rounded-lg text-left">
                        <div class="h-2 bg-sky-300 rounded-t-md"></div>
                    <div class="py-6 px-8">
                        <input type="text" placeholder="Email/notelp" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none rounded-md">
                        <input type="password" placeholder="Password" class=" border w-full h-5 px-3 py-5 mt-2 hover:outline-none rounded-md">
                        <div class="flex justify-center items-baseline">
                            <button class="mt-4 bg-gray-600 hover:bg-red-400 border-double text-white py-2 px-6 rounded-lg">Login</button>
                        </div>
                        <div class="flex justify-center items-baseline">
                            <a href="#" class="text-sm hover:underline">Forgot password?</a>
                        </div>
                        <div class="flex justify-center">
                            <a class="mx-2 text-gray-900" href=""> Atau </a>
                        </div>
                        <div class="flex justify-center items-baseline bg-green-600 border-8 border-green-500">
                             <a href="#" class="text-sm hover:underline hover:text-white">Register new account?</a>
                        </div>

                    </div>
                </div>
                <div>
                </div>
            </div>
        </div>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: form-login
</route>