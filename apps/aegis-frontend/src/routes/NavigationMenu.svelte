<script lang="ts">
  let collapsed = false;

  function toggle() {
    collapsed = !collapsed;
  }
</script>

<div class="navigation {collapsed ? '-collapsed' : ''}">
  <div class="navigation__brand">
    <h3>AEGIS</h3>
  </div>
  <div class="navigation__menu">
    <nav class="navigation__menu-items">
      <div class="navigation-item">
        <span class="navigation-item__icon" />
        <div class="navigation-item__text">Dashboard</div>
      </div>
      <div class="navigation-item">
        <span class="navigation-item__icon" />
        <div class="navigation-item__text">Suppliers</div>
      </div>
      <div class="navigation-item">
        <span class="navigation-item__icon" />
        <div class="navigation-item__text">Customers</div>
      </div>
      <div class="navigation-item">
        <span class="navigation-item__icon" />
        <div class="navigation-item__text">Products</div>
      </div>
      <div class="navigation-item">
        <span class="navigation-item__icon" />
        <div class="navigation-item__text">Stock</div>
      </div>
      <div class="navigation-item">
        <span class="navigation-item__icon" />
        <div class="navigation-item__text">Storage</div>
      </div>
    </nav>
  </div>
  <div class="navigation__actions">
    <button on:click={toggle}>{collapsed ? '>' : '<'}</button>
  </div>
</div>

<style lang="scss">
  .navigation {
    background-color: #f5f5f5;
    border-right: 1px solid #d6d6d6;

    height: 100vh;
    flex: 0;
    flex-basis: 300px;
    display: flex;
    flex-direction: column;
    transition: flex-basis 0.2s ease-in-out;

    &.-collapsed {
      flex-basis: 70px;

      // TODO: nested selectors without '&''
      .navigation__brand,
      .navigation-item__text {
        width: 0;
        overflow: hidden;
        opacity: 0;
        margin: 0;
      }

      .navigation__actions {
        text-align: center;
      }
    }

    &__brand {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 70px;
    }

    &__menu {
      flex: 1;
    }

    &__menu-items {
      padding: 1.5rem;
      display: flex;
      flex-direction: column;
    }

    &__actions {
      align-self: flex-end;
      padding: 0.5rem;
    }
  }

  .navigation-item {
    display: flex;
    cursor: pointer;
    text-align: center;
    width: 100%;

    &__text {
      opacity: 1;
      width: fit-content;
      margin-left: 1rem;
    }
  }
</style>
