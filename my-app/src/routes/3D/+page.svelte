<svelte:head>
	<title>3D Works</title>
	<meta name="description" content="3D Works Page" />
</svelte:head>

<script lang>
	import beret_dark from '$lib/images/2d/beret-girl-dark.png'
    import flower_wall from '$lib/images/2d/flower-wall.jpg'
    import georgia from '$lib/images/2d/georgia.png'
    import girl_purple from '$lib/images/2d/girl-purple.png'
    import hotel from '$lib/images/2d/hotel.png'
    import living_room from '$lib/images/2d/living-room.png'
    import poses from '$lib/images/2d/poses.png'
    import restaurant from '$lib/images/2d/restaurant.png'
    import sxr from '$lib/images/2d/sxr.png'
</script>

<p>
    3D works
</p>

<div class="gallery">
    <div class="art-col">
        <img src={restaurant} alt="Art" />
        <img src={girl_purple} alt="Art" />
        <img src={georgia} alt="Art" />
    </div>
    <div class="art-col">
        <img src={beret_dark} alt="Art" />
        <img src={flower_wall} alt="Art" />
        <img src={hotel} alt="Art" />
    </div>
    <div class="art-col">
        <img src={living_room} alt="Art" />
        <img src={sxr} alt="Art" />
        <img src={poses} alt="Art" />
    </div>
</div>

<style>
	img {
        align-self: center;
        width: 100%;
        margin: 3%;
	}

    .gallery {
        /* margin: 15% 4% 15% 4%; */
        display: flex;
        flex-direction: row;
		justify-content: center;
        /* flex: 0.2;
		align-items: center; */
    }

    .art-col {
        /* margin: 15% 4% 15% 4%; */
        display: flex;
        flex-direction: column;
		justify-content: top;
        width: 100%;
        flex: 0.3;
        margin: 1%;
		/* align-items: center; */
    }
</style>
