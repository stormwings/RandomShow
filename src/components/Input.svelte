<script>
  export let value = ""
</script>

<main>
  <input type="text" bind:value={value}>
  {value}
</main>