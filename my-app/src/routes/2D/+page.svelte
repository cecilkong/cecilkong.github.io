<svelte:head>
	<title>2D Works</title>
	<meta name="description" content="2D Works Page" />
</svelte:head>

<script lang>
	import beret_dark from '$lib/images/2d/beret-girl-dark.png'
    import beret_light from '$lib/images/2d/beret-girl-light.png'
    import dragon_expressions from '$lib/images/2d/dragon-expressions.png'
    import flower_wall from '$lib/images/2d/flower-wall.jpg'
    import georgia from '$lib/images/2d/georgia.png'
    import girl_purple from '$lib/images/2d/girl-purple.png'
    import hotel from '$lib/images/2d/hotel.png'
    import living_room from '$lib/images/2d/living-room.png'
    import poses from '$lib/images/2d/poses.png'
    import restaurant from '$lib/images/2d/restaurant.png'
    import sxr from '$lib/images/2d/sxr.png'

    import fig_1 from '$lib/images/2d/fig-1.jpg'
    import fig_2 from '$lib/images/2d/fig-2.jpg'
    import fig_3 from '$lib/images/2d/fig-3.jpg'
    import fig_4 from '$lib/images/2d/fig-4.jpg'
    import fig_5 from '$lib/images/2d/fig-5.jpg'
    import fig_6 from '$lib/images/2d/fig-6.jpg'

    import skater from '$lib/images/2d/skater-girl.png'
    import dragon from '$lib/images/2d/dragon.png'
    import goat from '$lib/images/2d/goat.png'
    import mouse from '$lib/images/2d/mouse.png'
    import jazz from '$lib/images/2d/jazz.png'
    import opera from '$lib/images/2d/opera.png'

    import { onMount } from 'svelte';
    import Modal from '../components/Modal.svelte';

    // let artworks = [
    // { id: 1, thumbnail: 'path-to-thumbnail1.jpg', fullSize: 'path-to-fullsize1.jpg' },
    // { id: 2, thumbnail: 'path-to-thumbnail2.jpg', fullSize: 'path-to-fullsize2.jpg' },
    // // Add more artwork objects
    // ];

    let selectedArt = null;

    function openModal(art) {
        selectedArt = art;
    }

    function closeModal() {
        selectedArt = null;
  }
</script>

<p class="intro">
    2D works
</p>

<p class="sub-section">
    personal
</p>
<div class="gallery">
    <div class="art-col pad-right">
        <img src={restaurant} alt="Art" />
        <img src={girl_purple} alt="Art" />
        <img src={georgia} alt="Art" />
    </div>
    <div class="art-col">
        <img src={beret_dark} alt="Art" />
        <img src={flower_wall} alt="Art" />
        <img src={hotel} alt="Art" />
    </div>
    <div class="art-col pad-left">
        <img src={living_room} alt="Art" />
        <img src={sxr} alt="Art" />
        <img src={poses} alt="Art" />
    </div>
</div>

<p class="sub-section">
    figure drawing
</p>
<div class="gallery">
    <div class="art-col pad-right">
        <img src={fig_1} alt="Art" />
        <img src={fig_2} alt="Art" />
    </div>
    <div class="art-col">
        <img src={fig_3} alt="Art" />
        <img src={fig_4} alt="Art" />
    </div>
    <div class="art-col pad-left">
        <img src={fig_5} alt="Art" />
        <img src={fig_6} alt="Art" />
    </div>
</div>

<style>
    .intro {
        font-size: 115%;
        font-weight: 900;
		margin: 10vh 0vw 0vh 0vw;
	}

    .sub-section{
        font-size: 105%;
        font-weight: 900;
		margin: 8vh 0vw 1vh 0vw;
	}

	img {
        align-self: center;
        width: 100%;
        margin: 3%;
	}

    .gallery {
        /* border-style: dotted; */
        display: flex;
        flex-direction: row;
		justify-content: center;
    }

    .art-col {
        /* border-style: dotted; */
        display: flex;
        flex-direction: column;
		justify-content: top;
        width: 100%;
        flex: 0.4;
    }

    .pad-left {
        padding-left: 1%;
    }

    .pad-right {
        padding-right: 1%;
    }
</style>
