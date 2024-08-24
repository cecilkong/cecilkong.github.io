<svelte:head>
	<!-- <title>Mango</title>
	<meta name="description" content="This is my home page." /> -->
</svelte:head>

<script lang="ts">
    import gma from '$lib/images/projects/shade-shift.png'
    import ProjectPage from '../../components/ProjectPage.svelte';
    let desc = 
        `Shift between the shades to navigate your way through 11 unique platforming puzzles filled 
        with both dexterity and strategy challenges. Each level consists of two shades of maps--both 
        are necessary to complete each level, but only one can be visible at a time. Balance between 
        thinking on your feet and planning ahead to reach the goal! 
        This game was created for a summer game prototyping class. I led a team of three people to 
        polish the prototype in three weeks. `;
</script>

<ProjectPage
    cover = {gma}
    role = "Programmer, level designer"
    tools = "Unity/C#, Git"
    timeline = "July 2022"
    team = "ten"
    description = {desc}
/>


<style>

</style>
