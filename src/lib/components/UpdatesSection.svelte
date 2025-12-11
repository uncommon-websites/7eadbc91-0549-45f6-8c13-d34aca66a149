<section class="py-20 border-b border-border">
	<div class="container-custom">
		<div class="grid grid-cols-1 md:grid-cols-2 gap-16">
			
			<!-- Left Column: CTA & Visual -->
			<div class="flex flex-col h-full">
				<div class="mb-8">
					<p class="font-mono text-xs text-muted mb-4">Start building</p>
					<h2 class="text-2xl font-medium mb-4">Production RAG without the pain</h2>
					<p class="text-muted font-light mb-8 text-sm leading-relaxed max-w-md">
						Built by engineers who spent three months rewriting RAG at NASA and Twitter. This is what we wish we had when we started.
					</p>
					<div class="flex gap-3 mb-12">
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							START FREE
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">S</span>
						</button>
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							VIEW DOCS
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">D</span>
						</button>
					</div>
				</div>
				
				<!-- Barcode Visual -->
				<div class="mt-auto w-full h-48 bg-black relative overflow-hidden flex items-center justify-center">
					{#each Array(100) as _, i}
						<div 
							class="h-full bg-white absolute" 
							style="
								left: {i}%; 
								width: {Math.random() * 2}%; 
								opacity: {Math.random()};
							"
						></div>
					{/each}
					<div class="absolute inset-0 flex items-center justify-center">
						<div class="bg-black text-white font-mono text-[10px] px-2 py-1 z-10">
							agentset.ai
						</div>
					</div>
				</div>
			</div>

			<!-- Right Column: Updates -->
			<div>
				<p class="font-mono text-xs text-muted mb-8">Latest updates</p>
				
				<div class="space-y-12">
					<!-- Update 1 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">January 15</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Agentset launches with production-grade RAG</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								After three months of rewriting RAG systems at NASA and Twitter, we're launching Agentset to spare other engineers this struggle. Production-ready hybrid search, reranking, and automatic citations in minutes, not months. Built for engineers who need accurate RAG but don't want to waste time optimizing retrieval quality.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Product Launch</span>
						</div>
					</div>

					<!-- Update 2 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">January 10</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Hybrid search: Why vector alone isn't enough</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								We learned the hard way that pure vector search fails on exact matches and technical terms. Our hybrid approach combines vector and keyword search automatically, delivering 89% accuracy on production workloads. No manual tuning required.
							</p>
							<div class="flex gap-2">
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Engineering</span>
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Best Practices</span>
							</div>
						</div>
					</div>

					<!-- Update 3 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">January 5</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Supporting 22+ file formats out of the box</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Agentset now supports PDF, DOCX, PPTX, XLSX, Markdown, CSV, images, and more. Built-in parsing and chunking strategies optimized for each format. Just upload your documents and start querying.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Feature Release</span>
						</div>
					</div>

					<!-- Update 4 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">December 20</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">From prototype to production: Our RAG journey</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								How we built one of the largest RAG systems (6B tokens, 9M pages) and why we had to rewrite every piece to achieve production quality. This is the story behind Agentset.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Company Story</span>
						</div>
					</div>
				</div>
			</div>

		</div>
	</div>
</section>
