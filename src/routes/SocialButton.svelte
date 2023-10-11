<script lang="ts">
	export let icon: string
	export let href: string
</script>

<a aria-labelledby={icon} {href} class="w-8 h-8" target="_blank">
	<img
		loading="lazy"
		class="hover:scale-125 aspect-square hover:rotate-3 duration-300"
		src={`/svg/${icon}.svg`}
		alt={icon}
		width="32"
		height="32"
	/>
</a>
