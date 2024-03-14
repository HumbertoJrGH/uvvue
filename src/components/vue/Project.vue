<template>
	<div class="project">
		<h2>{{ project.title }}</h2>
		<p>{{ project.description }}</p>
		<ul>
			<li v-for="tech in project.technologies" :key="tech">{{ tech }}</li>
		</ul>
	</div>
</template>

<script setup>
import { ref } from "vue"
const project = ref({
	title: "This is a title.",
	description: "This is a description.",
	technologies: ["Vue.js", "Astro.js", "typescript", "JavaScript", "HTML", "CSS"]
})
</script>

<style scoped>
.project {
	background-color: black;
	width: 500px;
	color: #ffffff66;
	padding: 1rem;
	border-radius: 1rem;
	margin-bottom: 20px;
}
</style>