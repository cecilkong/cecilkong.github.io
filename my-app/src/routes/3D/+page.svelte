<svelte:head>
	<title>3D Works</title>
	<meta name="description" content="3D Works Page" />
</svelte:head>

<script lang>
	import idle from '$lib/images/3d/idle.gif'
    import walk from '$lib/images/3d/walk.gif'
    import run from '$lib/images/3d/run.gif'
    import attack from '$lib/images/3d/attack.gif'
    import special from '$lib/images/3d/special.gif'
    import death from '$lib/images/3d/death.gif'
    import damaged from '$lib/images/3d/damage.gif'
    import jump from '$lib/images/3d/jump.gif'
    import env_1 from '$lib/images/3d/env-1.png'
    import env_2 from '$lib/images/3d/env-2.png'
    import env_3 from '$lib/images/3d/env-3.png'
    import env_video from '$lib/images/3d/duck.mp4'
    import fireplace from '$lib/images/3d/final-portfo.mp4'
</script>

<p class="intro">3D works</p>
<p>modeling, vfx, animation</p>

<div class="gallery">
    <div class="vfx">
        <p>VFX</p>
        <!-- <img src={fireplace} alt="Art" /> -->
        <img src={special} alt="Art" />
        <p>Animation, greenscreen, rotoscopes, color grading, particles, and final composite done with NukeX. 
            Flame VFX made in Maya. Models used under CC. 2024</p>
    </div>

    <div class="modeling">
        <p>Low Poly Environment</p>
        <img src={special} alt="Art" />
        <!-- <img src={env_video} alt="Art" /> -->
        <img src={env_1} alt="Art" />
        <img src={env_2} alt="Art" />
        <img src={env_3} alt="Art" />
    </div>

    <div class="animation">
        <p>Character Moveset</p>
        <img src={idle} alt="Art" />
        <img src={walk} alt="Art" />
        <img src={attack} alt="Art" />
        <img src={special} alt="Art" />
        <img src={jump} alt="Art" />
        <img src={death} alt="Art" />
        <img src={damaged} alt="Art" />
        <img src={run} alt="Art" />
    </div>
</div>

<style>
    .intro {
		margin: 10vh 0vw 0vh 0vw;
	}

    .gallery {
        display: flex;
        flex-direction: column;
		justify-content: center;
    }

    .vfx {
        border-style: dotted;
        align-self: flex-start;
    }

    .modeling {
        border-style: dotted;
    }

    .animation {
        border-style: dotted;
        align-self: flex-end;
    }

    /* .art-col {
        display: flex;
        flex-direction: column;
		justify-content: top;
        width: 100%;
        flex: 0.4;
        margin: 1%;
    } */
</style>
