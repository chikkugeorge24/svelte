<script>
  let count = 0;
  const handleClick = (event) => {
    console.log(event);
    count += 1;
  };
  const handleClickWithParams = (event, stepSize) => {
    console.log(event);
    count += stepSize;
  };
</script>

<main>
  <!--Inline event handlers-->
  <button on:click={() => (count = count + 1)}>Count {count}</button>

  <!--Using event handling function-->
  <button on:click={handleClick}>Count {count}</button>

  <!--Event handling function with parameters-->
  <button on:click={(event) => handleClickWithParams(event, 5)}
    >Count {count}</button
  >
  <button on:click={(event) => handleClickWithParams(event, 10)}
    >Count {count}</button
  >
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
