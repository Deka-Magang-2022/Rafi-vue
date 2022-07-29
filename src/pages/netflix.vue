<script setup lang="ts">
	useHead({
		title: 'Netflix',
	});
	
</script>

<template>
	<div class="-m-8 grid gap-2 bg-cover h-screen" style="background-image: url('https://assets.nflxext.com/ffe/siteui/vlv3/c2578c37-8569-4f88-b8f1-67a26a9ddcdd/2e83f3ab-d9d1-4f3a-81cb-2bb62aee8b5f/ID-id-20220725-popsignuptwoweeks-perspective_alpha_website_large.jpg')">
		<div class="min-h-screen bg-local place-content-center bg-gradient-to-b from-black via-black/50 to-black">
			<nav class="w-full py-4 px-8 flex items-center">
				<div class="font-serif text-5xl font-semibold text-red-600">NETFLIX</div>

				<div class="ml-auto  flex items-center h-full space-x-3">
					<select class="rounded-sm bg-transparent border-1 hover: py-2 border-white text-white after:content-[^] text-white font-semibold">
						<option value="" class="bg-gray-500">Bahasa Indonesia</option>
						<option value="" class="bg-gray-500">English</option>
					</select>
					<a href="#" class="border border-black bg-red-600 text-white font-[arial] hover:bg-red-400 rounded-sm px-4 py-2">Sign In
					</a>
				</div>
			</nav>
			<div class="grid place-content-center h-screen py-10">

				<section class="text-white text-center font-medium font-[arial]">
				<h1 class=" text-5xl font-semibold p-5 text-white">Unlimited movies, TV shows,
				<br> and more.</h1>
				<p class="text-2xl p-5">Watch anywhere. Cancel anytime.</p>
				<p class="text-xl p-4">Ready to watch? Enter your email to create or restart your membership.</p>
				</section>

				<section class="flex flex-row place-content-center">
					<input type="text" placeholder="Email Address" class="w-[525px] h-[60px]">	
					<button type="submit" class="transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110  duration-300 bg-red-700 w-[200px] h-[60px] text-white font-[arial]  hover:bg-red-400">GET STARTED ></button>
				</section>
			</div>

			
		</div>
		<div class="grid grid-row-6 gap-2  bg-gray-700">
			<div class="grid gap-2 bg-gray-800 text-white">
    <section class="flex justify-between bg-black h-[477px]">
      <section class="ml-40 mt-40 place-content-center">
        <p class="text-5xl mb-9">Enjoy on your TV.<br /></p>
        <p class="text-2xl mt-4">
          Watch on Smart TVs, Playstation, Xbox,<br />
          Chromecast, Apple TV, Blu-ray players, and <br />
          more.
        </p>
      </section>
      <img
        class="mr-48 w-[400px] h-96 mt-20"
        src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/tv.png"
        alt=""
        srcset=""
      />
    </section>
			

		</div>
		<section class="flex justify-between bg-black h-[460px]">
      <img
        class="w-[400] h-96 mt-20 ml-20"
        src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/mobile-0819.jpg"
        alt=""
      />
      <section class="mr-40 mt-40 place-content-center text-white">
        <p class="text-5xl mb-9">Download your shows <br />to watch offline.</p>
        <p class="text-2xl mt-4">
          Save your favorites easily and always have<br />
          something to watch. <br />
        </p>
      </section>
     </section>
     <section class="flex justify-between bg-black h-[535px]">
      <section class="ml-40 mt-40 place-content-center text-white">
        <p class="text-5xl mb-9">Watch everywhere.<br /></p>
        <p class="text-2xl mt-4">
          Stream unlimited movies and TV shows on<br />your phone, tablet, laptop, and TV.
          <br />
          more.
        </p>
      </section>
      <img
        src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/device-pile-id.png"
      />
     </section>
     <section class="flex justify-between bg-black h-[525px]">
      <img
        src="https://occ-0-64-58.1.nflxso.net/dnm/api/v6/19OhWN2dO19C9txTON9tvTFtefw/AAAABfpnX3dbgjZ-Je8Ax3xn0kXehZm_5L6-xe6YSTq_ucht9TI5jwDMqusWZKNYT8DfGudD0_wWVVTFLiN2_kaQJumz2iivUWbIbAtF.png?r=11f"
      />
      <section class="mr-40 mt-40 place-content-center text-white">
        <p class="text-5xl mb-9">Create profiles for kids.<br /></p>
        <p class="text-2xl mt-4">
          Send kids on adventures with their favorite<br />characters in a space made just
          for them—<br />free with your membership.
        </p>
      </section>
     </section>
     <section class="text-center bg-black h-[970px] text-white">
      <h1 class="text-5xl font-semibold mt-16">Frequently Asked Questions</h1>
      <section class="text-left flex place-content-center">
        <div class="text-3xl place-items-start flex flex-col gap-2 mt-6 p">
          <button class="bg-gray-700 text-left w-[890px] h-[80px] p-6">
            What is Netflix?
          </button>
          <button class="bg-gray-700 text-left w-[890px] h-[80px] p-6">
            How much does Netflix cost?
          </button>
          <button class="bg-gray-700 text-left w-[890px] h-[80px] p-6">
            Where can I watch?
          </button>
          <button class="bg-gray-700 text-left w-[890px] h-[80px] p-6">
            How do I cancel?
          </button>
          <button class="bg-gray-700 text-left w-[890px] h-[80px] p-6">
            What can I watch on Netflix?
          </button>
          <button class="bg-gray-700 text-left w-[890px] h-[80px] p-6">
            Is Netflix good for kids?
          </button>
		  <div class="text-white my-20 text-center">
				<p class="text-xl  py-3">Ready to watch? Enter your email to create or restart your membership.
				</p>
			<section class="flex flex-row place-content-center">
			<input type="text" placeholder="Email Address" class="w-[525px] h-[60px]">	
			<button type="submit" class="transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110  duration-300 bg-red-700 w-[200px] h-[60px] text-white font-[arial]  hover:bg-red-400">GET STARTED ></button>
			</section>
		  </div>
        </div>
      </section>
     </section>
     <div class="bg-black h-[426px] px-64 pt-[70px] text-gray-700">
					<div class="mb-8 text-white">
						<p>Questions? Call <a href="">007-803-321-2130</a></p>
					</div>
					<div class="grid grid-cols-4 grid-rows-4 gap-4 text-white">
						<p> FAQ </p>
						<p>Help Center</p>
						<p>Account</p>
						<p>Media Center</p>
						<p>Investor Relations</p>
						<p>Jobs</p>
						<p>Redeem Gift Cards</p>
						<p>Buy Gift Cards</p>
						<p>Ways to Watch</p>
						<p>Terms of Use</p>
						<p>Privacy</p>
						<p>Cookie Preferences</p>
						<p>Corporate Information</p>
						<p>Contact Us</p>
						<p>Speed Test</p>
						<p>Legal Notices</p>
						<p>Only on Netflix</p>
					</div>
					<div class="pt-5 ">
						<select name="" id="" class="py-1 border-gray-700 bg-black text-white">
							<option value="">English</option>
							<option value="">Indonesia</option>
						</select>
					</div>
					<div class="py-6 text-white">
						<p>Netflix Indonesia</p>
			
					</div>
				</div>
 			</div>
		</div>

</template>


					




		
			


					

