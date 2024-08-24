<svelte:head>
	<!-- <title>Mango</title>
	<meta name="description" content="This is my home page." /> -->
</svelte:head>

<script lang="ts">
    import gma from '$lib/images/projects/gma-green.png'
    import ProjectPage from '../../components/ProjectPage.svelte';
    let desc = 
        `Grandma Green is a virtual pet and farming simulation mobile game. 
        Play as a lonely Grandma who dreams of growing a beautiful garden, and in the process, 
        brings fruit, flower, and vegetable golems to life with her magic green thumb! 

This game was created over the course of two semesters with a 37-student team. `;
</script>

<ProjectPage
    cover = {gma}
    role = "Concept & UI Artist"
    tools = "Clip Studio Paint"
    timeline = "June 2022 - May 2023"
    team = "ten"
    description = {desc}
/>


<style>

</style>
