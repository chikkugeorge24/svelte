<script>
  import { setContext } from "svelte";
  import ComponentC from "./components/ComponentC.svelte";
  const userName = "chikku";
  setContext("username-context", userName);
</script>

<main>
  <h2>App component username - {userName}</h2>
  <ComponentC />
</main>

<style>
  main {
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
