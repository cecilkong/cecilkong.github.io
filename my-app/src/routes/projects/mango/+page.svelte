<svelte:head>
	<title>Mango Goes To Mewsic School</title>
	<meta name="description" content="Project page for Mango Goes To Mewsic School" />
</svelte:head>

<script lang="ts">
    import mango from '$lib/images/mgms/kpop-hitnotes.gif'
    import ProjectPage from '../../components/ProjectPage.svelte';
    let desc = 
        `Mango Goes to Mewsic School is a 2D rhythm-based RPG. Play as Mango, a young kitten who sets out 
                to learn the principles of four diverse genres—afrobeats, jazz, classical, and kpop—to pursue their 
                dream of going to music school.
                <br/>
                <br/>
                This game was created over the course of a semester with co-developer 
                Kaya Cook, a team of six Berklee students, and two usability partners. 
                <br/> 
                <br/>
                Winner of the Diversity in Video 
                Games Competition at the Congressional Black Caucus Foundation's 2023 Legislative Conference, sponsored 
                by the Entertainment Software Association. Read more here.`;
</script>

<ProjectPage
    name = "Mango Goes To Mewsic School"
    cover = {mango}
    role = "Co-Developer"
    tools = "Unity, Perforce, JetBrains Rider, Clip Studio Paint"
    timeline = "Jan 2023 - May 2023"
    team = "10"
    description = {desc}
/>

<div>
    <p>As a <strong>programmer</strong>, I implemented</p>
    <ul>
        <li>rhythm game mechanics & loop (dice rolling, score system,
            metronome, scrolling notes, measure bars, hit effects, corrupt notes, 
            particle effects)
            </li>
        <li>animations for the player, NPCs, and several other assets</li>
        <li>audio manager for music & sfx</li>
        <li>map layouts & obstacles for two worlds</li>
    </ul>
</div>

<div>
    <p>As an <strong>artist</strong>, I implemented</p>
    <ul>
        <li>concept art</li>
        <li>player character & NPCS</li>
        <li>UI assets (menus, dialogue, health, etc)</li>
        <li>environmental/decor assets</li>
        <li>character and environmental animations</li>
        <li>tilemap</li>
    </ul>
</div>

<div>
    <p>
        As co-developers, my partner and I were heavily involved in multiple other 
        processes in the creation of this game, including shared roles in
    </p>
    <ul>
        <li>level/map design</li>
        <li>narrative</li>
        <li>playtesting & collecting metrics</li>
        <li>overall production & scheduling</li>
    </ul>
</div>

<div>
    <p>Some tools and methods we used include</p>
    <ul>
        <li>a burndown chart</li>
        <li>agile development</li>
        <li>a game design macro</li>
        <li>playtest spreadsheet & questionnaires</li>
    </ul>
</div>


<style>

</style>
