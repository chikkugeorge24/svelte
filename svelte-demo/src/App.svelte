<script>
  import { shuffle } from "lodash";
  let names = ["Alan", "Alex", "David", "Mathew"];
  const shuffleNames = () => {
    names = shuffle(names);
  };
</script>

<main>
  {#each names as name (name)}
    <h2>{name}</h2>
    <input placeholder="Last name" />
  {/each}
  <div>
    <button on:click={shuffleNames}>Shuffle</button>
  </div>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
