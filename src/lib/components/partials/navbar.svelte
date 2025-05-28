<script>
	import NavbarLink from './navbar-link.svelte';
	import { base } from '$app/paths';
</script>

<nav class="bg-primary text-primary-foreground flex justify-between">
	<NavbarLink url="{base}/" testo="Home" />

	<div>
		<NavbarLink url="{base}/chi-siamo" testo="Chi siamo" />
		<NavbarLink url="{base}/impatto" testo="Impatto" />
		<NavbarLink url="{base}/programma" testo="Programma" />
		<NavbarLink url="{base}/eventi" testo="Eventi" />
		<NavbarLink url="{base}/unisciti-a-noi" testo="Unisciti a noi!" />
	</div>
</nav>
