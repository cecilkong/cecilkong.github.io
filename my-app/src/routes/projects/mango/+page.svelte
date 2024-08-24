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
                 dream of going to music school. This game was created over the course of a semester with co-developer 
                 Kaya Cook, a team of six Berklee students, and two usability partners. Winner of the Diversity in Video 
                 Games Competition at the Congressional Black Caucus Foundation's 2023 Legislative Conference, sponsored 
                 by the Entertainment Software Association. Read more here.`;
</script>

<ProjectPage
    name = "Mango Goes To Mewsic School"
    cover = {mango}
    role = "Co-Developer"
    tools = "Unity, Perforce, JetBrains Rider, Clip Studio Paint"
    timeline = "Jan - May 2023"
    team = "ten"
    description = {desc}
/>


<style>

</style>
