<svelte:head>
	<title>Home</title>
	<meta name="description" content="This is my home page." />
</svelte:head>

<script lang>
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
	<div class="proj-container">
		<div class="proj-thumbnail">
			<img src={mango} alt="Mango Goes To Mewsic School Thumbnail" />
		</div>
		<div class="proj-desc">
			<p>mango goes to mewsic school</p>
			<p>co-developer</p>
			<p>january 2023 - june 2023</p>
		</div>
	</div>

	<div class="proj-container">
		<div class="proj-thumbnail">
			<img src={gma_green} alt="Grandma Green Thumbnail" />
		</div>
		<div class="proj-desc">
			<p>grandma green</p>
			<p>concept artist</p>
			<p>june 2022 - may 2023</p>
		</div>
	</div>

	<div class="proj-container">
		<div class="proj-thumbnail">
			<img src={saleblazers} alt="Saleblazers Thumbnail" />
		</div>
		<div class="proj-desc">
			<p>saleblazers</p>
			<p>gameplay programming intern</p>
			<p>may 2023 - july 2023</p>
		</div>
	</div>

	<div class="proj-container">
		<div class="proj-thumbnail">
			<img src={shade_shift} alt="Shade Shift Thumbnail" />
		</div>
		<div class="proj-desc">
			<p>shade shift</p>
			<p>programmer, designer</p>
			<p>july 2022</p>
		</div>
	</div>

	<div class="proj-container">
		<div class="proj-thumbnail">
			<img src={scare_crow} alt="Scare Crow Thumbnail" />
		</div>
		<div class="proj-desc">
			<p>scare crow</p>
			<p>programmer, artist</p>
			<p>june 2024 - present</p>
		</div>
	</div>
</div>


<style>
	img {
        align-self: center;
        width: 100%;
		/* height: 37%; */
        /* margin: 3%; */
		/* overflow: hidden; */
	}

    .proj-container
    {
        display: flex;
        flex-direction: row;
		/* justify-content: space-between; */
		border-style: dotted;
		background-color: #E5E4E4;
    }

    .proj-thumbnail
    {
		width: 65%;
		height: 220px;
		overflow: hidden;
		border-style: dotted;

    }

	.proj-desc
    {
		border-style: dotted;
		width: 35%;
		text-align: end;

        margin: 0% 2% 0% 2%;
        /* display: flex;
        flex-direction: column;
		justify-content: top;
        width: 100%;
        flex: 0.3;
        margin: 1%; */
		/* align-items: center; */
    }
</style>
