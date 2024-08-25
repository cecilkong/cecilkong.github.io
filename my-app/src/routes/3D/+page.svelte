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
    <div class="row-section">
        <p class="section-title">VFX</p>
        <!-- <img src={fireplace} alt="Art" /> -->
         <div class="vfx">
            <img class="vfx-vid" src={special} alt="Art" />
            <p class="vfx-desc">Animation, greenscreen, rotoscopes, 
                color grading, particles, and final composite done with NukeX. 
                Flame VFX made in Maya. Models used under CC. 2024</p>
        </div>
    </div>

    <div class="row-section">
        <p class="section-title">Low Poly Environment</p>
        <div class="modeling">
            <div class="env">
                <p class="env-desc">Animation, greenscreen, rotoscopes, 
                    color grading, particles, and final composite done with NukeX. 
                    Flame VFX made in Maya. Models used under CC. 2024</p>
                <div class="env-vid">
                    <img src={special} alt="Art" />
                    <!-- <img src={env_video} alt="Art" /> -->
                </div>
            </div>
            <div class="env-photos">
                <img src={env_1} alt="Art" />
                <img src={env_2} alt="Art" />
                <img src={env_3} alt="Art" />
            </div>
        </div>
    </div>

    <div class="row-section">
        <p class="section-title">Character Moveset</p>
        <div class="anim">
            <div class="anim-col left">
                <img src={idle} alt="Art" />
                <img src={walk} alt="Art" />
                <img src={attack} alt="Art" />
            </div>
            <div class="anim-col">
                <img src={special} alt="Art" />
                <img src={jump} alt="Art" />
                <img src={death} alt="Art" />
            </div>
            <div class="anim-col">
                <img src={damaged} alt="Art" />
                <img src={run} alt="Art" />
            </div>
        </div>
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
    
    .row-section {
        /* border-style: dotted; */
        margin: 3vh 0vw 7vh 0vw;
    }

    .section-title {
        margin-bottom: 3%;
    }

    .vfx {
        display: flex;
        flex-direction: row;
    }

    .vfx-desc {
        /* border-style: dotted; */
        margin: 0vh 0vw 0vh 3vw;
    }

    /* .vfx-vid {
        border-style: dotted;
    } */

    .modeling {
        display: flex;
        flex-direction: column;
    } 

    .env 
    {
        /* border-style: dotted; */
        display: flex;
        flex-direction: row;
    }

    .env-desc {
        /* border-style: dotted; */
        margin: 0vh 3vw 0vh 0vw;
    }

    .env-photos {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin-top: 3%;
    }

    .env-photos img {
        width: 32%;
    }

    .anim {
        /* border-style: dotted; */
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .anim-col {
        /* border-style: dotted; */
        display: flex;
        flex-direction: column;
        width: 32%;
    }

    .anim-col img {
        margin-bottom: 5%;
    }
</style>
