<script>
  import Card from "./components/Card.svelte";
  import NameList from "./components/NameList.svelte";
</script>

<main>
  <!-- <Card>Card Content</Card>
  <Card>
    <h2>Card Content</h2>
  </Card>
  <Card>
    <img src="https://picsum.photos/200" alt />
  </Card>
  <Card /> -->

  <Card>
    <div slot="header">
      <h2>Card Header</h2>
    </div>
    <div slot="content">
      <img src="https://picsum.photos/200" alt />
    </div>
    <!-- <div slot="footer">
      <button>View Details</button>
    </div> -->
  </Card>

  <NameList>
    <h2 slot="hero" let:firstName let:lastName>{firstName} {lastName}</h2>
  </NameList>

  <NameList>
    <h2 slot="hero" let:firstName let:lastName>{lastName} {firstName}</h2>
  </NameList>

  <NameList>
    <h2 slot="hero" let:firstName let:lastName>{firstName}</h2>
  </NameList>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
