<section class="py-20 border-b border-border">
	<div class="container-custom">
		<div class="flex flex-col md:flex-row justify-between items-start mb-16 gap-8">
			<div>
				<h2 class="text-3xl font-medium mb-2">Superior RAG accuracy out of the box</h2>
				<p class="text-xl text-muted font-light">Production-ready retrieval quality without months of optimization</p>
			</div>
			<div class="max-w-xs text-[10px] text-muted leading-relaxed border-l border-border pl-4">
				<strong class="text-foreground block mb-1">About this benchmark</strong>
				This benchmark measures retrieval accuracy across 1,000 real-world queries spanning technical documentation, research papers, and enterprise knowledge bases. Each query requires precise context retrieval and citation accuracy. Results show Agentset's hybrid search and reranking delivering production-grade accuracy. Learn more in our <a href="#" class="underline">documentation</a>.
			</div>
		</div>

		<div class="relative w-full h-[500px] border border-border bg-primary-50/30 p-8 font-mono text-xs">
			<!-- Chart Grid -->
			<div class="absolute inset-0 p-8 grid grid-rows-6 grid-cols-1">
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
			</div>
			
			<!-- Y Axis Label -->
			<div class="absolute left-2 top-1/2 -translate-y-1/2 -rotate-90 text-muted origin-center whitespace-nowrap">
				ACCURACY (%)
			</div>

			<!-- X Axis Label -->
			<div class="absolute bottom-2 left-1/2 -translate-x-1/2 text-muted">
				COST (CPM)
			</div>

			<!-- Top Left Legend -->
			<div class="absolute top-4 left-4 flex gap-4 text-[10px] text-muted">
				<span class="bg-gray-200 px-1 rounded text-foreground">RAG-Bench</span>
				<span>Enterprise Knowledge</span>
				<span>Technical Docs</span>
				<span>Citation Accuracy</span>
			</div>

			<!-- Data Points -->
			
			<!-- Agentset (The Winner) -->
			<div class="absolute top-[12%] left-[18%] flex flex-col items-center group cursor-pointer z-10">
				<div class="flex items-center gap-2 mb-1">
					<span class="text-accent font-bold">AGENTSET</span>
				</div>
				<div class="w-3 h-3 bg-accent rounded-full shadow-[0_0_0_4px_rgba(255,68,0,0.2)]"></div>
				<div class="mt-1 text-[10px] text-accent">89% / $0.01/page</div>
			</div>

			<!-- Vectara -->
			<div class="absolute top-[35%] left-[40%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-100">
					<span class="font-bold text-[10px]">VECTARA</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">72% / $0.015/page</div>
			</div>

			<!-- LlamaIndex -->
			<div class="absolute top-[55%] left-[35%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-100">
					<span class="font-bold text-[10px]">LLAMAINDEX</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">65% / DIY</div>
			</div>

			<!-- Langchain -->
			<div class="absolute top-[65%] left-[30%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-100">
					<span class="font-bold text-[10px]">LANGCHAIN</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">58% / DIY</div>
			</div>

			<!-- Basic Vector Search -->
			<div class="absolute top-[78%] right-[25%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-100">
					<span class="font-bold text-[10px]">BASIC VECTOR</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">48% / DIY</div>
			</div>

			<!-- Bottom Right Legend -->
			<div class="absolute bottom-4 right-4 flex items-center gap-4 text-[10px]">
				<div class="flex items-center gap-1">
					<div class="w-2 h-2 bg-accent rounded-full"></div>
					<span class="text-accent font-bold">AGENTSET</span>
				</div>
				<div class="flex items-center gap-1">
					<div class="w-2 h-2 bg-black rounded-full"></div>
					<span class="text-muted">COMPETITORS</span>
				</div>
			</div>
		</div>
	</div>
</section>
