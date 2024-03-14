<template>
	<div class="dashboard">
		<h1>Dashboard</h1>
		<p>This is a simple Vue Dashboard built with Astro.js!</p>
		<Project />
	</div>
</template>

<script setup>
import Project from "./Project.vue"
</script>

<style>
.dashboard {
	margin: 0 auto;
	max-width: 1024px;
}
</style>