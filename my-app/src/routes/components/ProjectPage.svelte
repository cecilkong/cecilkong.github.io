<svelte:head>
	<title>{name}</title>
	<meta name="description" content="Project page for Mango Goes To Mewsic School">
</svelte:head>

<script>
    export let name;
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
	img {
        align-self: center;
        width: 100%;
        max-height: 400px;
	}

    .proj-page {
		border-style: dotted;
		background-color: #E5E4E4;
        margin: 2vh 2vw 2vh 2vw;
    }

    .summary {
        display: flex;
        flex-direction: row;
    }

    .stats {
		border-style: dotted;
        align-self: flex-start;
		width: 40%;
    }

	.description {
		border-style: dotted;
        align-self: flex-end;
		width: 60%;
    }
</style>