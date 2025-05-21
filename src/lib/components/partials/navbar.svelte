<script>
	import NavbarLink from './navbar-link.svelte';
</script>

<nav class="bg-primary text-primary-foreground flex justify-between">
	<NavbarLink url="/" testo="Home" />

	<div>
		<NavbarLink url="/chi-siamo" testo="Chi siamo" />
		<NavbarLink url="/impatto" testo="Impatto" />
		<NavbarLink url="/programma" testo="Programma" />
		<NavbarLink url="/eventi" testo="Eventi" />
		<NavbarLink url="/unisciti-a-noi" testo="Unisciti a noi!" />
	</div>
</nav>
