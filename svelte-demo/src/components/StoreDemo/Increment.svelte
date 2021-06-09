<script>
  import { count } from "../../store/stores";
  const increment = () => {
    count.update((curr) => {
      return curr + 1;
    });
  };
</script>

<button on:click={increment}>Increment</button>
