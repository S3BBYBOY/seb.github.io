<script lang="ts">
	const portfolioImages = [
		{
			alt: "Joining Webinar to gain more knowledge ",
			src: "Portfolio/8-bit-clarity.jpg",
		},
		{
			alt: "Application Development Blog project",
			src: "Portfolio/blogproject.jpg",
		},
		{
			alt: "Application Development Blog projec",
			src: "Portfolio/blogproject1.jpg",
		},
		{
			alt: "Latest sports ",
			src: "Portfolio/bowling.jpg",
		} 
	];
</script>

<h1 class="text-4xl text-center">Portfolio</h1>
<p class="text-center mb-8">Here are my Project, Activities and Sports that I have worked on:</p>
<div class="w-full max-w-4xl mx-auto">
    <div class="grid gap-8 grid-cols-1 md:grid-cols-2">
        {#each portfolioImages as portfolioImage (portfolioImage.src)}
        <div class="w-full h-fit overflow-hidden rounded-lg text-center">
            <img 
                src={portfolioImage.src} 
                alt={portfolioImage.alt} 
                class="w-full h-80 object-contain hover:scale-110 transition-transform duration-300 mx-auto" 
            >
            <p class="mt-4 text-lg">{portfolioImage.alt}</p>
        </div>
        {/each}
    </div>
</div>