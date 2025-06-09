<svelte:head>
	<title>Scare Crow</title>
	<meta name="description" content="Project page for Scare Crow" />
</svelte:head>

<script lang="ts">
    import scare_crow from '$lib/images/projects/sc1.png'
    import ProjectPage from '../../components/ProjectPage.svelte';
    let desc = 
        `wip scarecrow`;
</script>

<ProjectPage
    name = "Scare Crow"
    cover = {scare_crow}
    role = "Programmer, Artist"
    tools = "Unity/C#, Perforce, Procreate"
    timeline = "June 2024 - Present"
    team = "ten"
    description = {desc}
/>


<style>

</style>
