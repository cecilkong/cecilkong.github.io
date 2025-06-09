<script lang="ts">
	export let image: string;
    export let gif: string;
	export let title;
	export let role;
    export let tools;
	export let time;
    export let page_link;
  
  let current_src = image;

  function handleMouseEnter() {
    current_src = gif;
  }

  function handleMouseLeave() {
    current_src = image;
  }

  function handleKeyDown(event: KeyboardEvent) {
    if (event.key === 'Enter' || event.key === 'Space') {
      current_src = current_src === image ? gif : image;
    }
  }
</script>

<a href={page_link}>
    <div 
        class="proj-container" 
        role="button" 
        tabindex="0" 
        on:keydown={handleKeyDown}
        aria-label="Image hover effect"
        on:mouseenter={handleMouseEnter} 
        on:mouseleave={handleMouseLeave}>
        <div class="proj-thumbnail">
            <img src={current_src} alt="{title} Thumbnail"/>
        </div>
        <div class="proj-desc">
            <div class="title">
                <p>{title}</p>
            </div>
            <div class="info">
                <p>{role}<br/>{tools}<br/>{time}</p>
            </div>
        </div>
    </div>
</a>

<style>
	img {
        align-self: center;
        width: 100%;
	}

    .proj-container {
        /* border-style: dotted; */
        display: flex;
        flex-direction: row;
		background-color: #E5E4E4;
        color: #000000; 
        transition: box-shadow 0.4s;
    }

    .proj-container:hover {
        /* border-style: dotted; */
        display: flex;
        flex-direction: row;
		background-color: #E5E4E4;
        box-shadow: 5px 5px 10px 0 rgb(150, 154, 172), 0 17px 50px 0 rgba(0, 0, 0, 0.196);
        transition: box-shadow 0.4s;
    }

    :global(body.dark-mode) .proj-container:hover {
        display: flex;
        flex-direction: row;
		background-color: rgb(30, 30, 34);
        box-shadow: 5px 5px 10px 0 rgb(0, 0, 0), 0 17px 50px 0 rgba(0, 0, 0, 0.196);
        transition: box-shadow 0.4s;
	}

    .proj-thumbnail {
        /* border-style: dotted; */
		width: 65%;
		height: 220px;
		overflow: hidden;
    }

    :global(body.dark-mode) .proj-container {
        background-color: rgb(30, 30, 34);
		color: #F1EDE7; 
	}

	.proj-desc {
        /* border-style: dotted; */
		width: 35%;
		text-align: end;
        margin: 1% 3% 1% 3%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        font-weight: 100;
        font-size: 90%;
    }

    .title {
        /* border-style: dotted; */
        font-weight: 900;
        font-size: 115%;
        /* color: rgb(0, 0, 0); */
    }
    /*
    .info {
        border-style: dotted;
    } */
</style>