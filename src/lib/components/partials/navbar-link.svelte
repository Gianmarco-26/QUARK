<script lang="ts">
	import { base } from '$app/paths';
	import { page } from '$app/state';

	type Attributi = {
		url: string;
		testo: string;
	};

	let a: Attributi = $props();

	const href = $derived(base + a.url);
	const isActive = $derived(href === page.url.pathname);
</script>

<a
	{href}
	class={[
		'block p-2',
		{
			'bg-primary text-primary-foreground hover:bg-tertiary hover:text-secondary-foreground':
				!isActive,
			'bg-secondary text-secondary-foreground': isActive
		}
	]}
>
	{a.testo}
</a>
