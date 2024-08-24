<svelte:head>
	<title>Home</title>
	<meta name="description" content="Home Page" />
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

<p class="intro">
	hi, i'm cecil. i code and draw.
</p>

<div class="projects">
	<div class="thumbnail">
		<ProjectThumbnail
			image={mango} 
			title="Mango Goes To Mewsic School" 
			role="Co-Developer" 
			time="January 2023 - June 2023" 
			page_link="/projects/mango"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={gma_green} 
			title="Grandma Green" 
			role="Concept Artist, UI Artist" 
			time="June 2022 - June 2023" 
			page_link="/projects/grandma-green"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={saleblazers} 
			title="Saleblazers" 
			role="Gameplay Programming Intern" 
			time="May 2023 - August 2023" 
			page_link="/projects/saleblazers"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={shade_shift} 
			title="Shade Shift" 
			role="Programmer, Designer" 
			time="July 2022" 
			page_link="/projects/shade-shift"
		/>
	</div>
	<div class="thumbnail">
		<ProjectThumbnail 
			image={scare_crow} 
			title="Scare Crow" 
			role="Gameplay Programmer" 
			time="June 2024 - Current" 
			page_link="/projects/scare-crow"
		/>
	</div>
</div>


<style>
	.intro {
		margin: 10vh 0vw 5vh 0vw;
	}

	.thumbnail {
		margin: 1% 0% 1% 0%;
	}

	:global(body) {
		background-color: #F1F1F1;
		color: #221D1A;
		transition: background-color 0.3s;
	}

	:global(body.dark-mode) {
		background-color: #221D1A;
		color: #F1F1F1;
	}
</style>
