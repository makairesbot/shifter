<template>
    <div id="game-border">
		<PlayerHPBar />
		<PlayerMPBar />
	</div>
</template>

<script setup lang="ts">
import PlayerHPBar from './components/PlayerHPBar.vue';
import PlayerMPBar from './components/PlayerMPBar.vue';


</script>

<style scoped>
#game-border {
	margin-top: 4px;
	width: fit-content;
	height: fit-content;
	min-width: 1280px;
	min-height: 720px;
	display: flex;
	flex-wrap: wrap;
	flex-direction: column;
	justify-content: top;
	align-items: center;
	outline: 1px solid rgb(0, 0, 0);
}

.top-bar-outline {
	width: 95%;
	height: 20px;
	border: 3px solid black;
	margin-top: 4px;
	background-color: rgb(95, 95, 95);
}
</style>
