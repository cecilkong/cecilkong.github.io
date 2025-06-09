<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=Kumbh+Sans:wght@100..900&family=Source+Code+Pro:ital,wght@0,200..900;1,200..900&display=swap" rel="stylesheet">

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
            <div class="label">
                <p class="title">ROLE</p>
                <p class="small">{role}</p>
            </div>
            <div class="label">
                <p class="title">TOOLS</p>
                <p class="small">{tools}</p>
            </div>
            <div class="label">
                <p class="title">TIMELINE</p>
                <p class="small">{timeline}</p>
            </div>
            <div class="label">
                <p class="title">TEAM</p>
                <p class="small">{team}</p>
            </div>
        </div>
        <div class="description">
            <!-- <p>{description}</p> -->
            <div>{@html description}</div>
        </div>
    </div>
</div>

<style>
    p {
        margin: 0;
    }

	img {
        align-self: center;
        width: 100%;
        max-height: 400px;
	}

    .label
    {
        margin-top: 0vh;
        margin-bottom: 2vh;
    }

    .title
    {
        font-weight: 600;
        font-size: 100%;
        color: rgb(167, 167, 167);
        font-family: "Kumbh Sans";
    }

    .small {
		font-size: 98%;
    }

    .proj-page {
		/* border-style: dotted; */
		/* background-color: #E5E4E4; */
        margin: 7vh 0vw 6vh 0vw;
    }

    .summary {
        display: flex;
        flex-direction: row;
        align-items: top;
        margin-top: 5vh;
        justify-content: space-between;
    }

    .stats {
		/* border-style: dotted; */
        align-self: flex-start;
		width: 30%;
    }

	.description {
		/* border-style: dotted; */
		width: 60%;
        font-family: var(--font-mono);
    }
</style>