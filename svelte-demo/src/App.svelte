<script>
  import PostList from "./components/PostList.svelte";
</script>

<main>
  <PostList />
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }
  :global(h3) {
    color: blue;
  }
</style>
