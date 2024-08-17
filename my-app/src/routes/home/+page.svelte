<svelte:head>
	<title>Home</title>
	<meta name="description" content="This is my home page." />
</svelte:head>

<script lang>
	import mango from '$lib/images/projects/mango.png'
    import gma_green from '$lib/images/projects/gma-green.png'
    // import shade_shift from '$lib/images/projects/ss.png'
    // import saleblazers from '$lib/images/projects/saleblazers.png'
    // import equinox from '$lib/images/projects/equinox.png'
    // import lechord from '$lib/images/projects/lechord.png'
</script>

<p>
	hi, i'm cecil. i code and draw.
</p>

<div class="projects">
	<div class="proj-container">
		<div class="proj-thumbnail">
			<img src={mango} alt="Mango Goes To Mewsic School Thumbnail" />
		</div>
		<div class="proj-desc">
			<p>mango</p>
			<p>co-developer</p>
			<p>january 2023 - june 2023</p>
		</div>
	</div>

	<div class="proj-container">
		<div class="proj-thumbnail">
			<img src={gma_green} alt="Grandma Green Thumbnail" />
		</div>
		<div class="proj-desc">
			<p>gma green</p>
			<p>concept artist</p>
			<p>june 2022 - may 2023</p>
		</div>
	</div>
</div>


<style>
	img {
        align-self: center;
        width: 100%;
        margin: 3%;
	}

    .proj-container
    {
        display: flex;
        flex-direction: col;
		justify-content: space-between;
		border-style: dotted;
    }

    .proj-thumbnail
    {
		width: 40%;
		border-style: dotted;
    }

	.proj-desc
    {
		border-style: dotted;
        /* margin: 15% 4% 15% 4%; */
        /* display: flex;
        flex-direction: column;
		justify-content: top;
        width: 100%;
        flex: 0.3;
        margin: 1%; */
		/* align-items: center; */
    }
</style>
