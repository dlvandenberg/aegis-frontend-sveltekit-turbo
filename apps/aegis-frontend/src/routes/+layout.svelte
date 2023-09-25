<script>
  import NavigationMenu from './NavigationMenu.svelte';
  import TopBar from './TopBar.svelte';
</script>

<div class="app-container">
  <NavigationMenu />
  <div class="main">
    <TopBar />
    <div class="content">
      <slot />
    </div>
  </div>
</div>

<style lang="scss">
  .app-container {
    display: flex;
    width: 100%;
    height: 100%;
  }

  .main {
    display: flex;
    flex-direction: column;
    flex: 1;
  }
</style>
