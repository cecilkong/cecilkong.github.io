<svelte:head>
	<title>Home</title>
	<meta name="description" content="This is my home page." />
</svelte:head>

<script lang="ts">
	// import pfp from '$lib/images/svelte-welcome.webp';
	import pfp_fallback from '$lib/images/pfp_fallback.jpg';

    let bio = 
        `I’m a senior studying <strong>Computer Science</strong> with an emphasis in games along with a minor in 
        <strong>3D Animation</strong> at the <strong>University of Southern California</strong>.
        While I am primarily interested in gameplay programming, I've been making digital art 
        for several years—I often contribute a mix of both programming and art in many of my projects, 
        so you'll see some of both highlighted here. Ultimately, regardless of the medium, 
        I am dedicated to bringing creative ideas to life! In my free time, I enjoy longboard dancing, 
        journaling, and listening to music.`;
</script>

<div class="text-column">
    <picture>
        <!-- <source srcset={welcome} type="image/webp" /> -->
        <img src={pfp_fallback} alt="About Photo" />
    </picture>

	<p>
		Hi, I'm Cecil.
	</p>

    <p>
        {@html bio}
	</p>
</div>

<style>
	img {
		/* display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6; */
        /* max-width: 10%;
        max-height: 10%; */
        height: 30%;
        width: 30%;
	}
</style>
