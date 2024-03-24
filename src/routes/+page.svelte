<script>
	import Button from '$lib/components/button.svelte';
	import NavLink from '$lib/components/nav-link.svelte';
	import NavLogo from '$lib/components/nav-logo.svelte';
	import Nav from '$lib/components/nav.svelte';
</script>

<Nav>
	<NavLogo slot="logo" />
	<NavLink href="#">Services</NavLink>
	<NavLink href="#">About</NavLink>
	<NavLink href="#">Contact</NavLink>
</Nav>
<main>
	<h1>Main Header</h1>
	<h2>Subheader</h2>

	<Button>Learn More</Button>
	<p class="primary-text">Primary Text</p>
	<p class="primary-text">
		Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam sed turpis leo. Maecenas
		sollicitudin, augue ut euismod laoreet, sapien mi imperdiet dolor, quis elementum nisl ex vitae
		leo. Cras vel tincidunt odio. Orci varius natoque penatibus et magnis dis parturient montes,
		nascetur ridiculus mus. Fusce viverra accumsan ante vitae mattis. Cras tristique nulla quis
		congue pretium. Integer maximus dui vel lorem feugiat, quis aliquet elit sollicitudin. Curabitur
		gravida leo ut augue faucibus rhoncus. Etiam congue elementum purus vitae semper. Cras malesuada
		mauris augue, id tempor lectus dictum et. Quisque porttitor malesuada eleifend. Vestibulum vel
		convallis augue, sit amet efficitur lectus. Nulla sed felis eget orci semper mollis. Fusce
		sapien lorem, ultricies sed dictum ultrices, faucibus a nunc. Proin condimentum massa cursus
		elementum dictum. Pellentesque eget sapien eget elit varius placerat quis quis quam.
	</p>
	<br />
	<p class="secondary-text">Secondary Text</p>
	<p class="secondary-text">
		Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam sed turpis leo. Maecenas
		sollicitudin, augue ut euismod laoreet, sapien mi imperdiet dolor, quis elementum nisl ex vitae
		leo. Cras vel tincidunt odio. Orci varius natoque penatibus et magnis dis parturient montes,
		nascetur ridiculus mus. Fusce viverra accumsan ante vitae mattis. Cras tristique nulla quis
		congue pretium. Integer maximus dui vel lorem feugiat, quis aliquet elit sollicitudin. Curabitur
		gravida leo ut augue faucibus rhoncus. Etiam congue elementum purus vitae semper. Cras malesuada
		mauris augue, id tempor lectus dictum et. Quisque porttitor malesuada eleifend. Vestibulum vel
		convallis augue, sit amet efficitur lectus. Nulla sed felis eget orci semper mollis. Fusce
		sapien lorem, ultricies sed dictum ultrices, faucibus a nunc. Proin condimentum massa cursus
		elementum dictum. Pellentesque eget sapien eget elit varius placerat quis quis quam.
	</p>

	<div class="swatch primary"></div>
	<div class="swatch accent"></div>
	<div class="swatch background-a"></div>
	<div class="swatch background-b"></div>
	<p class="text-a">This is normal text</p>
	<p class="text-b">This is light text</p>
	<p class="text-a">
		This is text with a <a href="#">link</a> in it
	</p>
</main>

<style lang="scss">
	@use '/src/lib/style/colors';

	:global(body) {
		font-family: 'mr-eaves-xl-sans', sans-serif;
		font-weight: 400;
		font-style: normal;
		font-size: 1.25rem;
		color: colors.$text-a;
		background: colors.$background-a;
		margin: 0;
	}

	main {
		margin: auto;
		padding: 2rem 0rem;
		max-width: 900px;
	}

	.primary-text {
		color: colors.$text-a;
	}

	.secondary-text {
		color: colors.$text-b;
	}

	.swatch {
		height: 50px;
		width: 200px;

		&.primary {
			background-color: colors.$primary;
		}

		&.accent {
			background-color: colors.$accent;
		}

		&.background-a {
			background-color: colors.$background-a;
		}

		&.background-b {
			background-color: colors.$background-b;
		}
	}

	.text-a {
		color: colors.$text-a;
	}

	.text-b {
		color: colors.$text-b;
	}

	a {
		color: colors.$text-b;

		&:hover {
			color: colors.$text-hover;
		}
	}
</style>
