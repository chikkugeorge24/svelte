<script>
  import { count, customCount } from "../../store/stores";
  // import { onDestroy } from "svelte";
  // let counter;
  // const unsubscribe = count.subscribe((value) => {
  //   counter = value;
  // });
  // onDestroy(unsubscribe);
</script>

<!--$ will do subscribe and unsubcribe operations-->
<h2>Current count is {$count}</h2>
<h2>The custom count is {$customCount}</h2>

<button on:click={() => customCount.increment()}>Increment</button>
<button on:click={() => customCount.increment(5)}>Increment 5</button>
<button on:click={() => customCount.decrement()}>Decrement</button>
<button on:click={() => customCount.decrement()}>Decrement 5</button>
<button on:click={() => customCount.reset()}>Reset</button>
