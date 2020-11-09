<template>
  <section class="main-hero">
    <div class="main-hero__box">
      <div class="main-hero__box02">
        <nuxt-link to="/" class="main-hero__button">判決画面へ</nuxt-link>
      </div>
      <p class="main-hero__visual">
        <img src="/images/cat_boss_gang.png" alt="ねこ法務局長" />
      </p>
      <p class="main-hero__text">
        ねこねこ法務局ほ〜むとはねこ生における様々な犯罪を裁くところである。わかったら判決画面にいくがいい
      </p>
    </div>
  </section>
</template>

<style scoped>
body {
  font-family: "M PLUS Rounded 1c", sans-serif;
}

.main-hero {
  padding: 0 20px;
  background: #32cd32 no-repeat center center / cover;
  min-height: 100vh;
}

.main-hero__box {
  margin: 0 auto;
  text-align: center;
  max-width: 800px;
  margin-bottom: 10rem;
}

.main-hero__visual img {
  max-width: 200px;
  margin-top: 1rem;
}

.main-hero__text {
  margin-top: 2.5rem;
}

.main-hero__box02 {
  padding-top: 130px;
  text-align: center;
}

.main-hero__button {
  padding: 55px;
  color: #ffffff;
  font-size: 2rem;
  text-decoration: none;
  border-radius: 93px;
  background: #32cd32;
  box-shadow: -17px -17px 40px #adff2f, 17px 17px 40px #7cfc00;
}
</style>
