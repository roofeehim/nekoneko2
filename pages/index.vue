<template>
  <section class="main-hero">
    <div class="main-hero__box">
      <div class="main-hero__box02">
        <nuxt-link to="/about" class="main-hero__button"
          >法務局について</nuxt-link
        >
      </div>
      <p class="main-hero__visual">
        <img src="/images/cat_boss_gang.png" alt="ねこ法務局長" />
      </p>
      <p class="main-hero__text">判決を言い渡す！！</p>
      <div class="main-hero__box02">
        <a @click="random()" class="main-hero__button">かくにん</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    random: function () {
      var results = [
        "有罪",
        "無罪",
        "最高裁で戦え",
        "今日は帰りなさい",
        "執行猶予3年",
        "ねこ労働10年",
        "無期限活動停止",
        "この判例は私にも判断しかねる",
      ];

      var result = Math.floor(Math.random() * results.length);

      alert(results[result]);
    },
  },
};
</script>

<style scoped>
body {
  font-family: "M PLUS Rounded 1c", sans-serif;
}

.main-hero {
  min-height: 100vh;
  padding: 0 20px;
  background: #32cd32 no-repeat center center / cover;
}

.main-hero__box {
  margin: 0 auto;
  text-align: center;
  max-width: 800px;
  padding-bottom: 10rem;
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
