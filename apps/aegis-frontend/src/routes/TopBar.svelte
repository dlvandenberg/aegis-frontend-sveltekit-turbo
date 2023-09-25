<header class="top-bar">
  <ul class="top-bar__items">
    <li class="top-bar__item">
      <span>LanguageChooser</span>
    </li>
    <li class="top-bar__item">
      <span>Notifications</span>
    </li>
    <li class="top-bar__item">
      <span>John Doe</span>
    </li>
    <li class="top-bar__item">
      <span>Logout</span>
    </li>
  </ul>
</header>

<style lang="scss">
  .top-bar {
    padding: 0 0.5rem;
    background-color: #f5f5f5;
    border-bottom: 1px solid #d6d6d6;
    height: 70px;
    align-items: center;

    &__items {
      list-style: none;
      display: flex;
      flex-direction: row;
      justify-content: flex-end;
    }

    &__item {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      margin-left: 0.5rem;
    }
  }
</style>
