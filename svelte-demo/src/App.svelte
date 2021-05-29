<script>
  import PopUp from "./components/PopUp.svelte";
  let showPopup = false;
  const closePopup = (event) => {
    showPopup = false;
    console.log(event.detail);
  };
</script>

<main>
  <button on:click={() => (showPopup = true)}>Open popup</button>
  {#if showPopup}
    <PopUp on:close={closePopup} />
  {/if}
</main>

<style>
  main {
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
