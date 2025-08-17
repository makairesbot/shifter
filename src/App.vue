<template>
    <div id="game-border">
		<PlayerHPBar />
		<PlayerMPBar />
		<div id="content-panels">
			<div class="column20">
				<OptionsPane />
				<StatsPane />
			</div>
			<div class="column30">
				<MovementActionsPane />
				<GeneralActionsPane />
			</div>
			<div class="column20">
				<QueuePane />
			</div>
			<div class="column30">
				<InventoryPane />
				<ActionHistoryPane />
			</div>
		</div>
	</div>
</template>

<script setup lang="ts">
import PlayerHPBar from './components/PlayerHPBar.vue';
import PlayerMPBar from './components/PlayerMPBar.vue';
import OptionsPane from './components/OptionsPane.vue';
import StatsPane from './components/StatsPane.vue';
import MovementActionsPane from './components/MovementActionsPane.vue';
import GeneralActionsPane from './components/GeneralActionsPane.vue';
import QueuePane from './components/QueuePane.vue';
import InventoryPane from './components/InventoryPane.vue';
import ActionHistoryPane from './components/ActionHistoryPane.vue';


</script>

<style>
#game-border {
	margin-top: 4px;
	width: fit-content;
	height: fit-content;
	min-width: 1280px;
	min-height: 720px;
	height: 100%;
	display: flex;
	flex-direction: column;
	justify-content: top;
	align-items: center;
	overflow: scroll;
}

#content-panels {
	width: 95%;
	margin-top: 8px;
	margin-bottom: 8px;
	min-height: 644px;
	height: 80%;
	display: flex;
	flex-direction: row;
	justify-content: space-between;
}

.column20 {
	width: 236px;
	min-height: 644px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.column30 {
	width: 356px;
	min-height: 644px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.top-bar-outline {
	width: 95%;
	height: 20px;
	border: 3px solid black;
	margin-top: 4px;
	background-color: rgb(95, 95, 95);
}
</style>
