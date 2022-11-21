<script lang="ts">
	import Header from 'ilojo-bar-components/components/Header.svelte';
	import Footer from 'ilojo-bar-components/components/Footer.svelte';
	import '../styles/style.css';
</script>

<Header />
<main>
	<slot />
</main>
<Footer companyName="Legacy" />
