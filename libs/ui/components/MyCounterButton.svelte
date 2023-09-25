<script lang="ts">
  let count = 0;

  function handleClick() {
    count += 1;
  }
</script>

<button on:click={handleClick}>
  clicks: {count}
</button>

<style lang="scss">
  button {
    background-color: #f5f5f5;
    border: 1px solid #d6d6d6;
    padding: 0.5rem 1rem;
    border-radius: 0.25rem;
    cursor: pointer;
  }
</style>
