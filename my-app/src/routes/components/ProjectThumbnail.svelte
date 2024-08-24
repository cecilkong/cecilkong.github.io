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

    .proj-container {
        /* border-style: dotted; */
        display: flex;
        flex-direction: row;
		background-color: #E5E4E4;
    }

    .proj-thumbnail {
        /* border-style: dotted; */
		width: 65%;
		height: 220px;
		overflow: hidden;
    }

    :global(.proj-container.dark-mode) {
		background-color: #221D1A;
		color: #F1EDE7;
	}

	.proj-desc {
        /* border-style: dotted; */
		width: 35%;
		text-align: end;
        margin: 1% 3% 1% 3%;
    }
</style>