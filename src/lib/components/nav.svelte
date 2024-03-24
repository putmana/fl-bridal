<script lang="ts">
	//
</script>

<nav>
	<div class="logo">
		<slot name="logo" />
	</div>
	<div class="links">
		<slot />
	</div>
</nav>

<style lang="scss">
	@use '/src/lib/style/colors';

	nav {
		height: 4rem;
		margin: 0;
		top: 0;
		left: 0;
		right: 0;
		background-color: colors.$background-a;
		border-bottom: 1px solid colors.$shadow-b;
		display: flex;
		padding: 0 2rem;
		align-items: center;

		.logo {
			flex-grow: 1;
		}

		.links {
			display: flex;
			justify-content: flex-end;
			gap: 1.5rem;
		}
	}
</style>
