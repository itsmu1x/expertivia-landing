<script lang="ts">
	import "../app.css"
	import SocialButton from "./SocialButton.svelte"

	const links: { icon: string; href: string }[] = [
		{ icon: "discord", href: "https://discord.gg/Gxb9EEnvts" },
		{ icon: "instagram", href: "https://instagram.com/expertivia" },
		{ icon: "telegram", href: "https://t.me/expertivia" },
		{ icon: "tiktok", href: "https://tiktok.com/@expertivia" },
		{
			icon: "github",
			href: "https://github.com/itsmu1x/expertivia-landing",
		},
	]
</script>

<!-- some styling.. ig? -->
<div class="w-52 sm:w-64">
	<img
		width="250"
		height="250"
		loading="lazy"
		src="/images/logo.png"
		alt="Expertivia"
		class="drop-shadow-2xl hover:scale-110 hover:rotate-2 duration-300"
	/>
	<h1 class="text-4xl mt-2 text-center">Expertivia</h1>
</div>

<div class="flex flex-wrap gap-3.5">
	{#each links as link (link.icon)}
		<SocialButton {...link} />
	{/each}
</div>
