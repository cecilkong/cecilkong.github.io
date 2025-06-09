<svelte:head>
	<title>About</title>
	<meta name="description" content="About Page" />
</svelte:head>

<script lang="ts">
	import pfp_fallback from '$lib/images/about/pfp-fallback.jpg';
</script>

<div class="about">
    <div class="photo">
        <img src={pfp_fallback} alt="About Photo" />
    </div>
    <div class="bio">
        <div class="text">
            <p class="name">
                <strong>Hi, I'm Cecil.</strong>
            </p>
            <p>
                I’m a senior studying <strong>Computer Science</strong> with an emphasis in games 
                at the <strong>University of Southern California</strong>.
                While I am primarily interested in gameplay programming, I've been making digital art
                for several years—I often contribute a mix of both programming and art in many of my projects,
                so you'll see some of both highlighted here. Ultimately, regardless of the medium,
                I am dedicated to bringing creative ideas to life! In my free time, I enjoy longboard dancing,
                journaling, and listening to music.
            </p>
        </div>

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
    strong {
        font-weight: 900;
        color:rgb(135, 156, 39);
        font-size: 105%;
    }

	img {
        width: 25vw;
	}

    .about {
        /* border-style: dotted; */
        width: 100%;
        margin-top: 12vh;
        margin-bottom: 12vh;
        display: flex;
        flex-direction: row;
    }

    .photo {
        /* border-style: dotted; */
        margin: auto 0vw auto 0vw;
        align-self: flex-start;
    }

    .bio {   
        /* border-style: dotted; */
        margin: 0vh 0vw auto 0vw;
        align-self: flex-end;
        margin-left: 5vw;
        font-weight: 100;
    }

    .text {
        /* border-style: dotted; */
        margin-top: 0vh;
        margin-bottom: 0vh;
    }

    .name {
        /* border-style: dotted; */
        margin-top: 0vh;
        margin-bottom: 0vh;
    }

    .links {
        /* border-style: dotted; */
        display: flex;
        flex-direction: column;
        width: 20vw;
    }

    a {
        border-style: solid;
        height: 2.2vh;
        background-color: rgb(135, 156, 39);
        border-color: rgb(135, 156, 39);
        color: #F1EDE7;
        margin: 0.5vh 0vw 0.5vh 0vw;
        padding: 1vh 1vw 1.5vh 1vw;
    }

    a:hover {
        border-style: solid;
        background-color: #F1EDE7;
        color: rgb(135, 156, 39);
        box-shadow: 5px 5px 10px 0 rgb(138, 146, 181), 0 17px 50px 0 rgba(0, 0, 0, 0.196);
    }

    /* .role 
    {
        font-size: 0.8em;
        color:rgb(138, 146, 181);
    } */
</style>
