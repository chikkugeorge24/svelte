<script>
  import { count } from "../../store/stores";
  // import { onDestroy } from "svelte";
  // let counter;
  // const unsubscribe = count.subscribe((value) => {
  //   counter = value;
  // });
  // onDestroy(unsubscribe);
</script>

<!--$ will do subscribe and unsubcribe operations-->
<h2>Current count is {$count}</h2>
