<script setup lang="ts">
import { ref } from 'vue';

defineProps<{ msg: string }>();
const count = ref(0);
const countchange = () => {
	count.value += 1;
};
</script>

<template>
	<h1>{{ msg }}</h1>

	<div class="card">
		<button type="button" @click="countchange">count is {{ count }}</button>
	</div>
</template>

<style scoped>
.read-the-docs {
	color: #888;
}
</style>
