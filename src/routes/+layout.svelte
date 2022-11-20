<script lang="ts">
	// import { Footer, Header } from 'ilojo-bar-components/components';
	import Header from 'ilojo-bar-components/components/Header.svelte';
	import Footer from 'ilojo-bar-components/components/Footer.svelte';
	import '../styles/style.css';
</script>

<Header />
<main>
	<slot />
</main>
<Footer companyName="Legacy" />
