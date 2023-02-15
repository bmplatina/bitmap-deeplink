<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";

</script>

<template>
  <header>
    <div class="wrapper">
      <h1><a href="//prodbybitmap.com">Bitmap</a></h1>
      <nav>
        <ul class="menu">
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><a href="//wiki.prodbybitmap.com">위키</a></li>
          <li><RouterLink to="/esd/games">게임</RouterLink></li>
          <li><a href="//esd.prodbybitmap.com">지원</a></li>
          <li><RouterLink to="/about">About</RouterLink></li>
        </ul>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
@import url('https://fonts.cdnfonts.com/css/helvetica-neue-9');
@import url('https://cdn.jsdelivr.net/npm/font-applesdgothicneo@1.0/all.min.css');

* {
  font-family: 'Helvetica Neue', 'Helvetica', 'AppleSDGothicNeo', 'Noto Sans KR', sans-serif;
}

header {
  height: 75px;
  backdrop-filter: blur(5px);
  background: linear-gradient(0deg, rgba(32, 32, 32, 0.75), rgba(32, 32, 32, 0.75));
  line-height: 75px;
  position: fixed;
  width: 100%;
  z-index: 999;
  top: 0;
  left: 0;
}

h1 {
  color: white;
  line-height: 75px;
  float: left;
}

.menu {
  float: right;
}

.menu li {
  float: left;
}

.menu a {
  line-height: 75px;
  color: white;
  padding: 0 15px;
}

.wrapper {
  width: 1170px;
  margin: 0 auto;
}
</style>
