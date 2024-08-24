<svelte:head>
	<!-- <title>Mango</title>
	<meta name="description" content="This is my home page." /> -->
</svelte:head>

<script lang="ts">
    import gma from '$lib/images/projects/scare-crow.png'
    import ProjectPage from '../../components/ProjectPage.svelte';
    let desc = 
        `wip scarecrow`;
</script>

<ProjectPage
    cover = {gma}
    role = "Programmer, Artist"
    tools = "Unity/C#, Perforce, Procreate"
    timeline = "June 2024 - Present"
    team = "ten"
    description = {desc}
/>


<style>

</style>
