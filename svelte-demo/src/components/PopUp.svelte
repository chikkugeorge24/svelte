<script>
  import { createEventDispatcher } from "svelte";
  const dispatch = createEventDispatcher();
</script>

<h2>This is a popup</h2>
<button on:click={() => dispatch("close", "Chikku")}>Close Popup</button>
