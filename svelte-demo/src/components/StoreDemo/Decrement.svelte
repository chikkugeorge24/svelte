<script>
  import { count } from "../../store/stores";
  const decrement = () => {
    count.update((curr) => {
      return curr - 1;
    });
  };
</script>

<button on:click={decrement}>Decrement</button>
