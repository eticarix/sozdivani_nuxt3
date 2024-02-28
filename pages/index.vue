<template>

	<div class="bg-gray-100 p-10 w-9/12 mx-auto   h-[400px] rounded-3xl shadow-2xl">
		<h1>İndex Page</h1>
		<p>Lorem, ipsum, dolor sit amet consectetur adipisicing elit. Minus, ratione quasi neque non, itaque inventore voluptatem ullam amet ab est, impedit accusantium cumque. Amet cumque, commodi sequi voluptate fugit, cum.</p>

		<p class="text-3xl text-rose-500 p-10 text-center">{{ mesaj }}</p>

		<button class="bg-slate-400 px-3 py-2 text-teal-400 cursor-pointer" @click="selamAL('aleykumselam')">Selam AL</button>
		<main-footer :data="mesaj" />
	</div>
</template>

<script setup>

	const mesaj = ref("S.a")  //-->state  sayfa içerisindeki kullanılan değişkenler

	setTimeout(() => {
		mesaj.value = "Selamun Aleykum"
	}, 2000)


	const selamAL = (val) => {
		mesaj.value = val
	}


</script>
<style>
	
</style>
