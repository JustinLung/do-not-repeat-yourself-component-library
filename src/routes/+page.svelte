<script lang="ts">
	import Window from 'ilojo-bar-components/components/Window.svelte';
	import WindowSection from 'ilojo-bar-components/components/WindowSection.svelte';
	import type { PageData } from './$types';

	export let data: PageData;
</script>

<WindowSection>
	{#each data.stories as story}
		<a href="/stories/{story.id}">
			<Window
				storyTitle={story.title}
				storyImage={story.thumbnail.url}
				altTag={story.thumbnail.title}
			/>
		</a>
	{/each}
</WindowSection>

<style>
	a {
		text-decoration: none;
		color: var(--color-white);
	}
</style>
