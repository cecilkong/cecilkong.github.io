<svelte:head>
	<!-- <title>Home</title> -->
	<!-- <meta name="description" content="This is my home page." /> -->
</svelte:head>

<script>
	export let cover;
	export let role;
	export let tools;
	export let timeline;
    export let team;
    export let description;
</script>

<div class="proj-page">
    <div class="cover">
        <img src={cover} alt="Game thumbnail" />
    </div>
    <div class="summary">
        <div class="stats">
            <p>ROLE</p>
            <p>{role}</p>
            <p>TOOLS</p>
            <p>{tools}</p>
            <p>TIMELINE</p>
            <p>{timeline}</p>
            <p>TEAM</p>
            <p>{team}</p>
        </div>
        <div class="description">
            <p>{description}</p>
        </div>
    </div>
</div>

<style>
    /* .cover {
        max-height: 30%;
    } */

	img {
        align-self: center;
        width: 100%;
        max-height: 400px;
	}

    .proj-page
    {
        /* display: flex; */
        /* flex-direction: row; */
		/* justify-content: space-between; */
		border-style: dotted;
		background-color: #E5E4E4;
        margin: 2vh 2vw 2vh 2vw;
    }

    .summary 
    {
        display: flex;
        flex-direction: row;
    }

    .stats
    {
		border-style: dotted;
        align-self: flex-start;
		width: 40%;
		/* text-align: end; */
        /* margin: 0% 2% 0% 2%; */
    }

	.description
    {
		border-style: dotted;
        align-self: flex-end;
		width: 60%;
		/* text-align: end; */
        /* margin: 0% 2% 0% 2%; */
    }
</style>