<script>
  import Button from "./components/Button.svelte";
  import Outer from "./components/Outer.svelte";
  const greetFunc = (event) => {
    alert(event.detail);
  };
  const buttonClick = () => {
    alert("clicked");
  };
</script>

<main>
  <Outer on:greet={greetFunc} />
  <Button on:click={buttonClick} />
</main>

<style>
  main {
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
