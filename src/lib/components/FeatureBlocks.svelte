<script lang="ts">
	import FeatureBlock from './FeatureBlock.svelte';
</script>

<!-- Block 1: Hybrid Search -->
<FeatureBlock 
	title="Hybrid search that just works" 
	description="Combines vector and keyword search automatically. No manual tuning required for production-grade retrieval."
	buttons={[
		{ text: "TRY IT FREE", icon: true },
		{ text: "READ DOCS" }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 font-mono text-xs">
		<div class="flex items-center gap-2 border-b border-border pb-2 mb-4">
			<span class="text-accent">></span>
			<span class="text-muted">Hybrid Search</span>
			<span class="w-2 h-4 bg-accent animate-pulse"></span>
		</div>
		<div class="space-y-3">
			<div class="flex items-center gap-2 text-[10px]">
				<div class="w-2 h-2 bg-primary-500 rounded-full"></div>
				<span class="text-muted">Vector: 0.89 relevance</span>
			</div>
			<div class="flex items-center gap-2 text-[10px]">
				<div class="w-2 h-2 bg-primary-600 rounded-full"></div>
				<span class="text-muted">Keyword: 0.92 relevance</span>
			</div>
			<div class="h-2 bg-gray-100 w-full rounded"></div>
			<div class="h-2 bg-gray-100 w-3/4 rounded"></div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 2: Automatic Reranking -->
<FeatureBlock 
	title="Built-in reranking for better results" 
	description="Automatically reranks retrieved documents to surface the most relevant context for your queries."
	buttons={[
		{ text: "SEE IT IN ACTION", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full max-w-md bg-white border border-border rounded shadow-sm p-6 flex flex-col gap-4">
		<div class="flex items-center gap-2 text-xs font-mono text-muted">
			<div class="w-4 h-4 border border-current rounded-sm flex items-center justify-center">
				<div class="w-2 h-2 bg-current rounded-[1px]"></div>
			</div>
			Reranking results...
		</div>
		<div class="w-full bg-gray-100 h-1.5 rounded-full overflow-hidden">
			<div class="bg-accent h-full w-2/3"></div>
		</div>
		<div class="flex gap-1">
			{#each Array(20) as _}
				<div class="w-1 h-3 bg-gray-200"></div>
			{/each}
		</div>
		<div class="mt-2 flex items-center gap-2 text-[10px] text-muted font-mono uppercase">
			<span class="w-3 h-3 border border-current rounded-full flex items-center justify-center">✓</span>
			OPTIMIZED
		</div>
	</div>
</FeatureBlock>

<!-- Block 3: Automatic Citations -->
<FeatureBlock 
	title="Automatic citation generation" 
	description="Every response includes verifiable citations with source attribution. Build trust with transparent, traceable answers."
	buttons={[
		{ text: "VIEW EXAMPLES", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>SOURCE</div>
			<div>RELEVANCE</div>
			<div>CITATION</div>
			<div>STATUS</div>
		</div>
		{#each [1, 2, 3, 4, 5, 6] as i}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="flex items-center gap-2">
					<div class="w-3 h-3 rounded-full bg-primary-400/20"></div>
					<span class="text-primary-600">Doc {i}</span>
				</div>
				<div class="text-muted">{95 - i * 3}%</div>
				<div class="h-1.5 w-8 bg-gray-100 rounded"></div>
				<div class="flex items-center gap-1">
					<div class="w-2 h-2 bg-green-500 rounded-full"></div>
					<span class="text-green-600">✓</span>
				</div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 4: Metadata Filtering -->
<FeatureBlock 
	title="Advanced metadata filtering" 
	description="Filter and refine results using custom metadata. Perfect for enterprise knowledge bases with complex taxonomies."
	buttons={[
		{ text: "EXPLORE FILTERS", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>DOCUMENT</div>
			<div>DEPARTMENT</div>
			<div>DATE</div>
			<div>SECURITY</div>
		</div>
		{#each [1, 2, 3, 4, 5, 6] as i}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="flex items-center gap-2">
					<div class="w-3 h-3 rounded-full bg-primary-400/20"></div>
					<span class="text-primary-600">File {i}</span>
				</div>
				<div class="text-muted text-[9px]">Engineering</div>
				<div class="text-muted text-[9px]">2024-01</div>
				<div class="h-1.5 w-8 bg-gray-200 rounded"></div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 5: Deep Research Mode -->
<FeatureBlock 
	title="Deep research mode for comprehensive answers" 
	description="Agentic reasoning built-in. Automatically explores multiple sources for thorough, well-researched responses."
	buttons={[
		{ text: "TRY DEEP RESEARCH", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 flex flex-col gap-4">
		<div class="flex items-center justify-between border-b border-border pb-2">
			<div class="text-[10px] font-mono text-muted flex items-center gap-2">
				<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
				Deep research in progress
			</div>
		</div>
		
		<!-- Research Progress Grid -->
		<div class="grid grid-cols-12 gap-1">
			{#each Array(48) as _, i}
				<div class="aspect-square rounded-[1px] {i < 32 ? 'bg-primary-500' : (i < 40 ? 'bg-primary-300' : 'bg-gray-50')}"></div>
			{/each}
		</div>

		<div class="mt-auto space-y-2">
			<div class="flex items-center gap-2 text-[10px] text-muted font-mono">
				<span class="w-3 h-3 border border-current rounded-full flex items-center justify-center text-[8px]">32</span>
				Sources analyzed
			</div>
			<div class="bg-gray-50 p-2 rounded border border-border flex gap-2 items-center">
				<div class="w-4 h-4 bg-primary-200 rounded"></div>
				<div class="h-1.5 w-24 bg-primary-100 rounded"></div>
			</div>
		</div>
	</div>
</FeatureBlock>
