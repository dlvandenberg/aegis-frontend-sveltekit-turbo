<script lang="ts">
  let open = false;

  function handleClick() {
    open = !open;
  }
</script>

<button on:click={handleClick}>
  Toggle: {open ? 'open' : 'closed'}
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
