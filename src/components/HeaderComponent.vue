<template>
  <header>
    <nav class="nav">
      <div class="nav__header">
        <div>
          <span> YGCORREA </span>
          <img class="code" src="../assets/code.png" />
        </div>
      </div>
      <div class="nav__links">
        <a> Hero </a>
        <a> About </a>
        <a> Services </a>
        <a> Skills </a>
        <a> Projects</a>
      </div>
      <div class="nav__button">
        <button class="large-button">Contact</button>
      </div>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  font-size: 2em;
  color: #a175e9;
  font-weight: 600;
}
.code {
  height: 30px;
}
.nav {
  height: 80px;
  display: flex;
  align-items: center;
  width: 100vw;
  justify-content: space-between;
  span {
    flex: 1;
    display: flex;
    justify-content: center;
  }
  a {
    color: #e9e9e9;
    font-size: 1rem;
    cursor: pointer;
    text-decoration: none;
    font-weight: 300;
    &:hover {
      color: #a175e9;
    }
  }
  &__links {
    flex: 1;
    display: flex;
    justify-content: space-between;
    @media (max-width: 767px) {
      display: none;
    }
  }
  &__button {
    flex: 1;
    display: flex;
    justify-content: center;
    @media (max-width: 767px) {
      display: none;
    }
  }
  &__header {
    display: flex;
    flex: 1;
    display: flex;
    justify-content: center;
    div {
      gap: 20px;
      display: flex;
      align-items: center;
    }
  }
}
</style>
