<svelte:head>
	<title>Home</title>
	<meta name="description" content="This is my home page." />
</svelte:head>

<script lang="ts">
	// import pfp from '$lib/images/svelte-welcome.webp';
	import pfp_fallback from '$lib/images/about/pfp-fallback.jpg';

    // let bio = 
    //     I’m a senior studying <span class="highlight"><strong>Computer Science</strong></span> with an emphasis in games along with a minor in 
    //     <strong><span class="highlight">3D Animation</span></strong> at the <strong>University of Southern California</strong>.
    //     While I am primarily interested in gameplay programming, I've been making digital art 
    //     for several years—I often contribute a mix of both programming and art in many of my projects, 
    //     so you'll see some of both highlighted here. Ultimately, regardless of the medium, 
    //     I am dedicated to bringing creative ideas to life! In my free time, I enjoy longboard dancing, 
    //     journaling, and listening to music.;
</script>

<div class="about">
    <div class="photo">
        <img src={pfp_fallback} alt="About Photo" />
    </div>
    <div class="bio">
        <p>
            <strong>Hi, I'm Cecil.</strong>
        </p>
        <p>
            <!-- {@html bio} -->
            I’m a senior studying <strong>Computer Science</strong> with an emphasis in games along with a minor in
            <strong>3D Animation</strong> at the <strong>University of Southern California</strong>.
            While I am primarily interested in gameplay programming, I've been making digital art
            for several years—I often contribute a mix of both programming and art in many of my projects,
            so you'll see some of both highlighted here. Ultimately, regardless of the medium,
            I am dedicated to bringing creative ideas to life! In my free time, I enjoy longboard dancing,
            journaling, and listening to music.
        </p>

        <!-- <p class="role">
            Current <br/>
            Gov Affairs Intern @ Entertainment Software Association (ESA) <br/>
            <br/>
            Prev. <br/>
            SWE Intern @ Ripple Effect Studios <br/> Gameplay Programming Intern @ Airstrafe Interactive
        </p> -->
        <div class="links">
            <a href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=cecil.lh.kong@gmail.com" 
            class="contact"
            target="_blank" 
            rel="noopener noreferrer">Email</a>

            <a href="https://www.linkedin.com/in/cecil-kong/" 
            class="contact"
            target="_blank" 
            rel="noopener noreferrer">LinkedIn</a>

            <a href="https://drive.google.com/file/d/1JlSx0UJEQ-WTTz6hQH1XO1DG52Kqhe1L/view?usp=drive_link" 
            class="contact"
            target="_blank" 
            rel="noopener noreferrer">Resume</a>
        </div>
    </div>
</div>

<style>
    strong 
    {
        font-weight: bolder;
        color:rgb(138, 146, 181)
    }

	img {
        width: 25vw;
	}

    .about
    {
        width: 100%;
        margin-top: 12vh;
        margin-bottom: 12vh;
        display: flex;
        flex-direction: row;
        /* border-style: dotted; */
    }

    .photo 
    {
        margin: auto 0vw auto 0vw;
        /* border-style: dotted; */
        align-self: flex-start;
    }

    .bio 
    {   
        margin: 0vh 0vw auto 0vw;
        /* border-style: dotted; */
        align-self: flex-end;
        margin-left: 5vw;
    }

    .links 
    {
        display: flex;
        flex-direction: column;
    }

    /* .contact  */
    a
    {
        border-style: solid;
        width: 20vw;
        background-color: rgb(138, 146, 181);
        border-color: rgb(138, 146, 181);
        color: #F1EDE7;
        margin: 0vh 0vw 1vh 0vw;
        padding: 1vh 1vw 1vh 1vw;
    }

    a:hover 
    {
        border-style: solid;
        background-color: #F1EDE7;
        color: rgb(138, 146, 181);
        box-shadow: 5px 5px 10px 0 rgb(138, 146, 181), 0 17px 50px 0 rgba(0, 0, 0, 0.196);
    }

    /* .role 
    {
        font-size: 0.8em;
        color:rgb(138, 146, 181);
    } */
</style>
