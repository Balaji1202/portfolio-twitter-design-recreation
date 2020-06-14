<template>
	<div class="main-panel">
		<div class="main-content">
			<p class="name-header">BALAJI SARAVANAN</p>
			<img class="header-image" src="./../assets/header-background.jpg" alt="">
		</div>
		<ExtrasPanel/>
	</div>
</template>

<script>
import ExtrasPanel from './ExtrasPanel.vue';
export default {
	components: {
		ExtrasPanel
	}
}
</script>

<style scoped>
	.main-panel {
		max-width: 600px;
		overflow: auto;
	}
	.main-content {

	}
	.header-image {
	}
</style>