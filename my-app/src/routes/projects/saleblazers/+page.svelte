<svelte:head>
	<title>Saleblazers</title>
	<meta name="description" content="Project page for Saleblazers" />
</svelte:head>

<script lang="ts">
    import saleblazers from '$lib/images/projects/saleblazers.png'
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
    name = "Saleblazers"
    cover = {saleblazers}
    role = "Gameplay Programming Intern"
    tools = "Unity/C#, Perforce, Visual Studio"
    timeline = "May 2023 - August 2023"
    team = "ten"
    description = {desc}
/>

<p>
    I worked on Saleblazers as Gameplay Programming Intern at Airstrafe Interactive during the 
    summer of 2023. My work ranged from implementing new features and creating tools for designers 
    to fixing bugs and refactoring old code.
</p>

<p>
    More specifically, I
</p>

<ul>
    <li>
    Developed an XP-soaking functionality for multiplayer gameplay using Unity Mirror networking, 
    enhancing player progression and engagement 
    </li>
    <li>
    Contributed to a significant refactoring of the audio system to determine all physics-based 
    sound effects, footstep and equipment foley, and weapon select and equip sound effects by object
    material, type, and size, enhancing audio realism and variety and resulting in a more immersive experience
    </li>
    <li>
    Programmed the combat music system to play, fade, and queue music tracks by enemy priority
    </li>
    <li>
    Created console commands for designers and QA testers to streamline the playtesting and bug-searching process
    </li>
    <li>
    Programmed custom Unity editor tools for gameplay and sound designers to easily adjust settings for new features 
    </li>
    <li>
    Fix various critical bugs, including audio, progression-blocking, cutscene, and networking bugs by 
    navigating a massive codebase with Visual Assist and Visual Studio debugger 
    </li>
</ul>
<style>

</style>
