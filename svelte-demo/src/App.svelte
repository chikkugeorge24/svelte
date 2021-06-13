<script>
  import Decrement from "./components/StoreDemo/Decrement.svelte";
  import Display from "./components/StoreDemo/Display.svelte";
  import Increment from "./components/StoreDemo/Increment.svelte";
  import Reset from "./components/StoreDemo/Reset.svelte";
  import Timer from "./components/StoreDemo/Timer.svelte";
</script>

<main>
  <Timer />
  <Display />
  <Increment />
  <Decrement />
  <Reset />
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }
  :global(h3) {
    color: blue;
  }
</style>
