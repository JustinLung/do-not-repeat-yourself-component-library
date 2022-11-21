<script lang="ts">
	import Window from 'ilojo-bar-components/components/Window.svelte';
	import WindowSection from 'ilojo-bar-components/components/WindowSection.svelte';
	import type { PageData } from './$types';

	export let data: PageData;
	console.log(data);
	const pageTitle = 'Stories';
</script>

<WindowSection>
	{#each data.stories as story}
		<Window
			storyTitle={story.title}
			storyImage={story.thumbnail.url}
			altTag={story.thumbnail.title}
		/>
	{/each}
</WindowSection>
