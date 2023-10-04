<template>
<div class="text-black p-4">© {{getYear}} hsiangting</div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
    let getYear = ref('');
	let day = new Date();
	getYear = day.getFullYear();
</script>