<script>
    export let selectedArt;
    import { createEventDispatcher } from 'svelte';
  
    const dispatch = createEventDispatcher();
  
    function close() {
      dispatch('close');
    }
</script>
  
  <div class="modal-overlay" on:click={close}>
    <div class="modal-content" on:click|stopPropagation>
      <img src={selectedArt.fullSize} alt="Full size art" class="fullsize-image" />
    </div>
  </div>
  
  <style>
    .modal-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.8);
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 1000;
    }
    .modal-content {
      position: relative;
      max-width: 90%;
      max-height: 90%;
    }
    .fullsize-image {
      max-width: 100%;
      max-height: 100%;
      object-fit: contain;
    }
  </style>