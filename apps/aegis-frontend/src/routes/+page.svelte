<script lang="ts">
  import { ToggleButton } from '@aegis/management';
  import { MyCounterButton } from '@aegis/ui';
</script>

<div class="container">
  <h1>Web</h1>
  <MyCounterButton />

  <hr />

  <ToggleButton />

  <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
</div>

<style lang="scss">
  .container {
    max-width: 600px;
    margin: 0 auto;
    padding: 1rem;
  }
</style>
