<script>
  import Greet from "./components/Greet.svelte";
  const name = "Chikku",
    channel = "Crafts Grimoire";
  const obj = {
    name: "Barry",
    heroName: "Flash",
  };
</script>

<main>
  <Greet name="William" heroName="Batman" />
  <Greet name="Clara" heroName="Wonderwomen" />
  <Greet name="Clark" heroName="Batman" />
  <Greet {name} />
  <Greet {...obj} />
</main>

<style>
  main {
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
