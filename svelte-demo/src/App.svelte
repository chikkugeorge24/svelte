<script>
  let firstName = "Chikku",
    lastName = "George";
  //Reactive declarations
  $: fullName = `${firstName} ${lastName}`;
  //Reactive statements
  $: {
    const greet = `${firstName} ${lastName}`;
    console.log(greet);
  }
  let items = [
    {
      id: 1,
      title: "TV",
      price: 100,
    },
    {
      id: 2,
      title: "Phone",
      price: 200,
    },
    {
      id: 3,
      title: "Laptop",
      price: 300,
    },
  ];
  $: total = items.reduce((total, cur) => (total = total + cur.price), 0);
  let volume = 0;
  $: if (volume < 0) {
    alert("Can not go lower");
    volume = 0;
  } else if (volume > 20) {
    alert("Can not go higher");
    volume = 20;
  }
</script>

<main>
  <h2>Current volume - {volume}</h2>
  <button on:click={() => (volume += 2)}>Increase Volume</button>
  <button on:click={() => (volume -= 2)}>Decrease Volume</button>

  <button
    on:click={() => {
      (firstName = "Clark"), (lastName = "Wane");
    }}
  >
    Change Name
  </button>
  <h2>{firstName} {lastName}</h2>
  <h2>{fullName}</h2>
  <button
    on:click={() =>
      (items = [...items, { id: 4, title: "Keyboard", price: 50 }])}
  >
    Add Items
  </button>
  <h2>
    Total - {total}
  </h2>
</main>

<style>
  main {
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
