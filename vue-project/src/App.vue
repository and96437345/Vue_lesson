<script setup>
import Card from './components/Card.vue'
</script>

<template>
  <div class="wrapper">
    <header class="header">
      <div class="container">
        <div class="header__row">
          <div class="header__logo logo">
            <div class="logo__image">
              <img src="./assets/logo.png" alt="" />
            </div>
            <div class="logo__right">
              <div class="logo__name">REACT SNEAKERS</div>
              <div class="logo__desc">Магазин лучших кроссовок</div>
            </div>
          </div>
          <div class="header__menu menu">
            <nav class="menu__nav">
              <ul class="menu__list">
                <li class="menu__item">
                  <a href="" class="menu__link">
                    <svg class="menu__icon menu__icon--card">
                      <use href="./assets/sprite.svg#icon-card"></use>
                    </svg>
                    1205 руб.</a
                  >
                </li>
                <li class="menu__item">
                  <a href="" class="menu__link">
                    <svg class="menu__icon">
                      <use href="./assets/sprite.svg#icon-heart"></use>
                    </svg>
                    Закладки</a
                  >
                </li>
                <li class="menu__item">
                  <a href="" class="menu__link">
                    <svg class="menu__icon">
                      <use href="./assets/sprite.svg#icon-lk"></use>
                    </svg>
                    Профиль</a
                  >
                </li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<style>
body {
  background: #e7f6ff;
  padding-top: 85px;
}
.wrapper {
  max-width: 1080px;
  margin: 0 auto;
  border-radius: 20px;
  background-color: #fff;
  box-shadow: 0px 10px 20px 0px rgba(0, 0, 0, 0.04);
  min-height: 90vh;
}
.container {
  max-width: 960px;
  margin: 0 auto;
  width: 96%;
}

.header {
  padding: 44px 0;
  border-bottom: 1px solid #eaeaea;
}
.header__row {
  display: flex;
  align-items: start;
  justify-content: center;
}
.logo {
  display: flex;
  align-items: center;
}
.logo__image {
  flex-shrink: 1;
  margin-right: 0;
}
.logo__name {
  color: #000;
  font-family: Inter;
  font-size: 20px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  text-transform: uppercase;
}
.logo__desc {
  color: #9d9d9d;
  font-family: Inter;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.menu__icon {
  height: 18px;
  width: 18px;
}
.menu__icon:not(.menu__icon--card) {
  fill: #9b9b9b;
}
</style>
