<template>
  <div id="app" class="app">
		<div class="col1">
			<NavigationPanel/>
		</div>
  </div>
</template>

<script>
import NavigationPanel from './components/NavigationPanel.vue'
export default {
  name: 'App',
  components: {
		NavigationPanel
  }
}
</script>

<style>
.app {
	display: flex;
	flex-direction: row;
	height: 100vh;
}
.col1 {
	width: 25%; 
}
.col2 {
	width: 45%;
}
.col3 {
	width: 30%;
}
.svg-theme-text {
	fill: black;
}
.svg-theme-background {
	fill: white;
}
.svg-theme-active {
	fill: rgb(29, 161, 242);
	transition: 0.5s;
}
@media (max-width: 1300px) {
	.col1 {
		width: 22.7rem;
		transition: 0.1s;
	}
}
@media (max-width: 1200px) {
	.col1 {
		width: 300px;
		transition: 0.1s;
	}
}
@media (max-width: 1100px) {
	.col1 {
		width: 80px;
		transition: 0.1s;
	}
}
@media (max-width: 450px) {
	.left-navigation {
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
		position: fixed;
		margin: 0;
		height: 60px;
		width: 100%;
		bottom: 0;
		overflow-y: hidden;
	}
	.sub-navs {
		display: none;
	}
}
</style>
