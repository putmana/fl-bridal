<script lang="ts">
	//
	export let href = '';
</script>

<a {href}>
	<slot />
</a>

<style lang="scss">
	@use '/src/lib/style/colors';

	a {
		transition: all 0.2s ease;
		color: colors.$text-a;
		text-transform: uppercase;
		font-weight: 600;
		text-decoration: none;

		&:hover {
			color: colors.$text-hover;
		}
	}
</style>
