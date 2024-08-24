<svelte:head>
	<title>Home</title>
	<meta name="description" content="This is my home page." />
</svelte:head>

<script lang>
	import ProjectThumbnail from '../components/ProjectThumbnail.svelte'
	import mango from '$lib/images/projects/mango.png'
    import gma_green from '$lib/images/projects/gma-green.png'
    import shade_shift from '$lib/images/projects/shade-shift.png'
    import saleblazers from '$lib/images/projects/saleblazers.png'
	import scare_crow from '$lib/images/projects/scare-crow.png'
    // import equinox from '$lib/images/projects/equinox.png'
    // import lechord from '$lib/images/projects/lechord.png'
</script>

<p>
	hi, i'm cecil. i code and draw.
</p>

<div class="projects">
	<div class="thumbnail">
		<ProjectThumbnail
			image={mango} 
			title="Mango Goes To Mewsic School" 
			role="Co-Developer" 
			time="january 2023 - june 2023" 
			page_link="/projects/mango"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={gma_green} 
			title="grandma green" 
			role="concept artist" 
			time="june 2022 - june 2023" 
			page_link="/projects/grandma-green"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={saleblazers} 
			title="saleblazers" 
			role="gameplay programming intern" 
			time="may 2023 - august 2023" 
			page_link="/projects/saleblazers"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={shade_shift} 
			title="shade shift" 
			role="programmer, designer" 
			time="july 2022" 
			page_link="/projects/shade-shift"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={scare_crow} 
			title="scare-crow" 
			role="gameplay programmer" 
			time="june 2024 - current" 
			page_link="/projects/scare-crow"
		/>
	</div>
</div>


<style>
	.thumbnail {
		margin: 1% 0% 1% 0%;
	}
	:global(body) {
		background-color: #F1EDE7;
		color: #221D1A;
		transition: background-color 0.3s
	}
	:global(body.dark-mode) {
		background-color: #221D1A;
		color: #F1EDE7;
	}
</style>
