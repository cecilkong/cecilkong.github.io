<svelte:head>
	<title>About</title>
	<meta name="description" content="About Page" />
</svelte:head>

<script lang="ts">
	import pfp from '$lib/images/about/pfp.jpeg';
</script>

<div class="about">
    <div class="photo">
        <img src={pfp} alt="About Photo" />
    </div>
    <div class="bio">
        <div class="text">
            <p class="name">Hi, I'm Cecil.</p>
            <p class="name">I'm a gameplay engineer.</p>
            <p class="desc">
                I graduated with a B.S. in <strong>Computer Science</strong> with an emphasis in games
                at the <strong>University of Southern California</strong>.
            </p>
            <p class="desc">
                Along with gameplay programming, I've been making digital art
                for several years—I often contribute both programming and art in many of my projects.
                Ultimately, regardless of the medium, I am dedicated to bringing creative ideas to life.
                In my free time, I enjoy longboard dancing, journaling, and listening to music.
            </p>
        </div>

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
        color:rgb(60, 91, 178);
        font-size: 102%;
    }

    :global(body.dark-mode) strong{
        font-weight: 900;
        color:rgb(166, 174, 198);
        font-size: 102%;
	}

	img {
        border-radius: 100%;
        width: 35vw;
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
        margin-left: 8vw;
        font-weight: 100;
        text-align: end;
    }

    .text {
        /* border-style: dotted; */
        margin-top: 0vh;
        margin-bottom: 0vh;
    }

    .desc 
    {
        font-family: var(--font-body);
        font-weight: 300;
        font-size: 100%;
    }

    .name {
        /* border-style: dotted; */
        font-style: italic;
        font-size: 125%;
        font-weight: 800;
        margin-top: 0vh;
        margin-bottom: 0vh;
    }

    .links {
        /* border-style: dotted; */
        display: flex;
        flex-direction: column;
        width: 13vw;
        justify-self: end;
    }

    a {
        border-style: solid;
        height: 2vh;
        background-color: rgb(166, 174, 198);
        border-color: rgb(166, 174, 198);
        color:black;
        /* border-color: black; */
        /* margin: 1vh 0vw 1vh 0vw;
        padding: 2vh 1vw 2vh 1vw; */
        margin: 1vh 0vw;
        padding: 1vh 1vw;
        border-radius: 10%;
        text-align: center;
    }

    :global(body.dark-mode) a{
        border-style: solid;
        height: 2vh;
        background-color: rgb(34, 49, 91);
        border-color: rgb(34, 49, 91);
        color:white;
        margin: 1vh 0vw;
        padding: 1vh 1vw;
        border-radius: 10%;
        text-align: center;
	}

    a:hover {
        border-style: solid;
        background-color: #F1EDE7;
        color:rgb(166, 174, 198);
        box-shadow: 5px 5px 10px 0 rgb(138, 146, 181), 0 17px 50px 0 rgba(0, 0, 0, 0.196);
    }

    :global(body.dark-mode) a:hover{
        border-style: solid;
        height: 2vh;
        background-color: rgb(0, 0, 0);
        border-color: rgb(0, 0, 0);
        margin: 1vh 0vw;
        padding: 1vh 1vw;
        border-radius: 10%;
        text-align: center;
	}
</style>
