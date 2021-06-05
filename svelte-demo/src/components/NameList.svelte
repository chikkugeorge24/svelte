<script>
  const names = [
    {
      firstName: "Alan",
      lastName: "Walker",
    },
    {
      firstName: "Jhoney",
      lastName: "Warner",
    },
    {
      firstName: "Louis",
      lastName: "Phelip",
    },
  ];
</script>

{#each names as name (name)}
  <slot name="hero" firstName={name.firstName} lastName={name.lastName} />
{/each}
