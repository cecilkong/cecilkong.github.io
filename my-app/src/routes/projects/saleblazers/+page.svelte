<svelte:head>
	<!-- <title>Mango</title>
	<meta name="description" content="This is my home page." /> -->
</svelte:head>

<script lang="ts">
    import gma from '$lib/images/projects/saleblazers.png'
    import ProjectPage from '../../components/ProjectPage.svelte';
    let desc = 
        `Saleblazers is an open-world multiplayer shopkeeping survival game where anything—from pistols to 
        chairs—can be sold at your store or wielded as a weapon. Build your own shop from scratch, fight off 
        dangerous monsters, and venture through a vast island. 
        I worked on Saleblazers as Gameplay Programming Intern at Airstrafe Interactive during the summer of 2023. 
        My work ranged from implementing new features and creating tools for designers to fixing bugs and refactoring 
        old code.`;
</script>

<ProjectPage
    cover = {gma}
    role = "Gameplay Programming Intern"
    tools = "Unity/C#, Perforce, Visual Studio"
    timeline = "May 2023 - August 2023"
    team = "ten"
    description = {desc}
/>


<style>

</style>
