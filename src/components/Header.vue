<template>
	<div class="wrapper">
		<header>
			<button @click="toggleNav()">Toggle</button>
		</header>
		<main>My Application</main>
	</div>
</template>
<script>
export default {
	name: "Header",
	methods: {
		toggleNav () {
			this.$parent.$emit('toggleNav')
		}
  }
}
</script>