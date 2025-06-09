<svelte:head>
	<title>Shade Shift</title>
	<meta name="description" content="Project page for Shade Shift" />
</svelte:head>

<script lang="ts">
    import ss from '$lib/images/projects/shade-shift.png'
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
    name = "Shade Shift"
    cover = {ss}
    role = "Programmer, level designer"
    tools = "Unity/C#, Git"
    timeline = "July 2022"
    team = "ten"
    description = {desc}
/>

Specifically, I

programmed map shifting & basic platforming mechanics including wall-jumping & sliding

led team meetings, organized milestones, assigned programming and design tasks, conducted playtests and compiled playtesting notes

designed and implemented 7 levels

<style>

</style>
