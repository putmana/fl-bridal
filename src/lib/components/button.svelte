<script lang="ts">
	//
</script>

<button>
	<slot />
</button>

<style lang="scss">
	@use '/src/lib/style/colors';
	button {
		transition: all 0.2s ease;
		background-color: transparent;
		border: 1px solid colors.$primary;
		color: colors.$text-a;
		font-family: inherit;
		font-size: 0.75rem;
		font-weight: 600;
		text-transform: uppercase;
		letter-spacing: 0.05em;
		padding: 1em;

		&:hover {
			color: colors.$background-a;
			background-color: colors.$primary;
			cursor: pointer;
		}
	}
</style>
