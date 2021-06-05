<script>
  import ChildStyles from "./components/ChildStyles.svelte";
</script>

<main>
  <h3>App Global component</h3>
  <h4>App Component</h4>
  <ChildStyles />
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
  h4 {
    color: orange;
  }
  :global(h3) {
    color: blue;
  }
</style>
