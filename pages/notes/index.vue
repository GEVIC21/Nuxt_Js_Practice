import { NewCard } from '../../.nuxt/components';
<template>
	<div>
		<h1>Notes</h1>
		<br>
        <button @click="boolean=!boolean">Add New {{ boolean }}</button>
        <br>
        <br>
		<NewNote/>
		<br>
        <NoteCard/>
		<!-- <div class="flex">
			<NoteCard v-for="n in 1" :key="n" :note="n"/>
		</div> -->
	</div>
</template>
<script setup>
const newNote =resolveComponent('NewNote');
const newCard =resolveComponent('newCard');

const boolean = ref(false);

</script>
<style scoped>
.flex {
	display: flex;
}
</style>
