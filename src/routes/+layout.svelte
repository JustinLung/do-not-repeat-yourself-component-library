<script lang="ts">
	import Link from 'ilojo-bar-components/components/Link.svelte';
	import Header from 'ilojo-bar-components/components/Header.svelte';
	import Footer from 'ilojo-bar-components/components/Footer.svelte';
	import '../styles/style.css';
</script>

<Header>
	<Link linkTitle="Home" link="/" />
	<Link linkTitle="About" link="/" />
</Header>
<main>
	<slot />
</main>
<Footer companyName="Legacy" />

<style>
	main {
		padding: 2rem 1rem;
	}
</style>
