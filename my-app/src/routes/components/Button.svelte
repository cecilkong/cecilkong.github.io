<script>
    function toggle() {
        window.document.body.classList.toggle('dark-mode')
    }
</script>

<button on:click={toggle}>
    <slot/>
</button>

<style>
    button {
        background-color: #F1F1F1;
        border: none;
        border-radius: 4px;
        padding: 0.5rem;
        transition: background-color 0.3s
    }

    button:hover {
        cursor: pointer;
    }

    :global(body) button {
        background-color: #F1F1F1;
        color: 131316;
        transition: background-color 0.3s;
    }

    :global(body.dark-mode) button {
        background-color: #131316;
        color: #F1F1F1;
        transition: background-color 0.3s;
    }
</style>