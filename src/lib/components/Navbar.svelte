<script lang="ts">
	import { onMount } from 'svelte';
	
	let showBanner = true;
</script>

{#if showBanner}
	<div class="bg-primary-50 border-b border-border py-2 px-4 text-xs font-mono flex justify-center items-center relative">
		<div class="flex items-center gap-2">
			<span class="text-muted">Production-ready RAG in minutes, not months.</span>
			<a href="#" class="underline decoration-muted hover:text-accent transition-colors">Get started free.</a>
		</div>
		<button 
			class="absolute right-4 text-muted hover:text-foreground"
			aria-label="Close banner"
			onclick={() => showBanner = false}
		>
			<svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path d="M9 3L3 9M3 3L9 9" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
			</svg>
		</button>
	</div>
{/if}

<nav class="border-b border-border bg-background sticky top-0 z-50">
	<div class="container-custom h-16 flex items-center justify-between">
		<!-- Logo -->
		<a href="/" class="text-xl font-bold tracking-tight flex items-center gap-2">
			<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-foreground">
				<path d="M4 4H20V20H4V4Z" stroke="currentColor" stroke-width="2"/>
				<path d="M8 4V20" stroke="currentColor" stroke-width="2"/>
				<path d="M16 4V20" stroke="currentColor" stroke-width="2"/>
				<path d="M4 12H20" stroke="currentColor" stroke-width="2"/>
			</svg>
			<span class="font-sans font-semibold">Agentset</span>
		</a>

		<!-- Links -->
		<div class="hidden md:flex items-center gap-8 font-mono text-xs text-muted">
			<a href="#" class="hover:text-foreground transition-colors">Features</a>
			<a href="#" class="hover:text-foreground transition-colors">Pricing</a>
			<a href="#" class="hover:text-foreground transition-colors">Docs</a>
			<a href="#" class="hover:text-foreground transition-colors">Blog</a>
			<a href="#" class="hover:text-foreground transition-colors">Careers</a>
		</div>

		<!-- CTA -->
		<div class="flex items-center gap-4">
			<a href="#" class="hidden md:flex items-center gap-2 border border-border px-3 py-1.5 text-xs font-mono hover:bg-primary-50 transition-colors uppercase">
				Start Building
				<svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M1 11L11 1M11 1H3M11 1V9" stroke="currentColor" stroke-width="1.5"/>
				</svg>
			</a>
			<div class="md:hidden">
				<!-- Mobile Menu Icon -->
				<svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
					<line x1="3" y1="12" x2="21" y2="12"></line>
					<line x1="3" y1="6" x2="21" y2="6"></line>
					<line x1="3" y1="18" x2="21" y2="18"></line>
				</svg>
			</div>
		</div>
	</div>
</nav>
