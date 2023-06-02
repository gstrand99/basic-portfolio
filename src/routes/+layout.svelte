<script lang='ts'>
	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-rocket.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell, AppBar, LightSwitch } from '@skeletonlabs/skeleton';
</script>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar>
			<svelte:fragment slot="lead">
				<strong class="text-xl uppercase"><a href="/">Garrett Strand</a></strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
        <LightSwitch />
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://linkedin.com/in/garrett-strand-b198a8208/"
					target="_blank"
					rel="noreferrer"
				>
					LinkedIn
				</a>
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://github.com/gstrand99"
					target="_blank"
					rel="noreferrer"
				>
					GitHub
				</a>
        <a
					class="btn btn-sm variant-ghost-surface"
					href="mailto:contact@garrett-strand.tech"
					target="_blank"
					rel="noreferrer"
				>
					Email
				</a>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
