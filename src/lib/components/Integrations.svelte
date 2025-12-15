<script lang="ts">
    // Simple SVG paths for icons would be better, but for now using colored squares/circles to mimic brand colors
    const integrations = [
        { name: 'Alibaba Cloud', color: 'bg-orange-500' },
        { name: 'SAP', color: 'bg-blue-500' },
        { name: 'Oracle', color: 'bg-red-600' },
        { name: 'Microsoft', color: 'bg-blue-600' },
        { name: 'Salesforce', color: 'bg-blue-400' },
        { name: 'ServiceNow', color: 'bg-green-700' },
        { name: 'AWS', color: 'bg-yellow-600' },
        { name: 'Azure', color: 'bg-blue-500' },
        { name: 'Google Cloud', color: 'bg-red-500' },
        { name: 'MongoDB', color: 'bg-green-600' },
        { name: 'PostgreSQL', color: 'bg-blue-700' },
        { name: 'MySQL', color: 'bg-blue-400' },
        { name: 'Redis', color: 'bg-red-500' },
        { name: 'Kafka', color: 'bg-gray-800' },
        { name: 'Docker', color: 'bg-blue-500' },
        { name: 'Kubernetes', color: 'bg-blue-600' }
    ];

    const security = [
        'Enterprise Security', 'Data Privacy', 'ISO 27001', 'Encryption', 
        'Access Control', 'Compliance', 'Audit Trails', 'Backup & Recovery', 
        'Network Security', 'API Security', 'Malaysian Data Laws', 'PDPA Compliant'
    ];
</script>

<section class="py-24 bg-black text-white">
	<div class="max-w-[1400px] mx-auto px-6 text-center">
		<h2 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6">
			Enterprise Integration<br />
			& Cloud Partnership
		</h2>
		<p class="text-gray-400 text-lg max-w-2xl mx-auto mb-20">
			Seamless integration with your existing systems, powered by Alibaba Cloud infrastructure for Malaysian enterprises.
		</p>

		<div class="grid grid-cols-1 lg:grid-cols-2 gap-20">
            <!-- Integrations -->
			<div>
                <div class="inline-block bg-primary-500 text-white text-[10px] font-bold px-3 py-1 rounded-full mb-8 tracking-wide uppercase">
                    Enterprise System Integration
                </div>
                
                <div class="grid grid-cols-4 gap-4">
                    {#each integrations as tool}
                        <div class="aspect-square bg-[#111] rounded-xl border border-white/5 flex flex-col items-center justify-center p-2 hover:bg-[#1a1a1a] transition-colors group">
                            <div class="w-8 h-8 rounded-lg {tool.color} mb-3 flex items-center justify-center opacity-80 group-hover:opacity-100 transition-opacity">
                                <!-- Simple icon placeholder -->
                            </div> 
                            <span class="text-[10px] text-gray-400 font-medium">{tool.name}</span>
                        </div>
                    {/each}
                </div>
            </div>

            <!-- Security -->
			<div>
                <div class="inline-block bg-primary-500 text-white text-[10px] font-bold px-3 py-1 rounded-full mb-8 tracking-wide uppercase">
                    Enterprise-Grade Security
                </div>
                
                <div class="grid grid-cols-4 gap-4">
                     {#each security as item}
                        <div class="aspect-square bg-[#111] rounded-xl border border-white/5 flex flex-col items-center justify-center p-2 hover:bg-[#1a1a1a] transition-colors group">
                            <div class="w-8 h-8 rounded-full border border-white/20 mb-3 flex items-center justify-center text-white/50 group-hover:text-white transition-colors">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                    <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/>
                                </svg>
                            </div> 
                            <span class="text-[10px] text-gray-400 text-center leading-tight font-medium">{item}</span>
                        </div>
                    {/each}
                </div>
            </div>
		</div>
	</div>
</section>
