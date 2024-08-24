<svelte:head>
	<!-- <title>Home</title> -->
	<!-- <meta name="description" content="This is my home page." /> -->
</svelte:head>

<script>
	export let image;
	export let title;
	export let role;
	export let time;
    export let page_link;
</script>

<a href={page_link}>
    <div class="proj-container">
        <div class="proj-thumbnail">
                <img src={image} alt="{title} Thumbnail" />
        </div>
        <div class="proj-desc">
            <p>{title}</p>
            <p>{role}</p>
            <p>{time}</p>
        </div>
    </div>
</a>

<style>
	img {
        align-self: center;
        width: 100%;
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
    }
</style>