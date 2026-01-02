<template>
  <header>
    <!-- <h1 class="hp-title"><router-link to="/">タイトル</router-link></h1> -->
    <nav>
      <ul>
        <li><a href="#top" class="nav-link">TOP</a></li>
        <li><span>/</span></li>
        <li><a href="#about-text" class="hover-line">About</a></li>
        <li><span>/</span></li>
        <li><a href="#skills" class="hover-line">Skills</a></li>
        <li><span>/</span></li>
        <li><a href="#works-list" class="hover-line">Works</a></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000; /* 前に出すため */
  display: flex;
  height: 50px;
}
h1 {
  font-size: 1.5em;
  line-height: 1.1;
  display: flex;
  align-items: center;
}

nav {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

nav ul {
  display: flex;
  gap: 2rem ;
  text-align: center;
  list-style: none;
}
nav a ,
.nav-link{
  color: rgb(0, 0, 0);
  text-decoration: none;
}
nav a.router-link-exact-active {
  font-weight: bold;
  border-bottom: 2px solid #fff;
}

/* タブレット → スマホ（必須） */
@media (max-width: 768px) {
  nav ul {
    gap: 1.5rem ;
}

}

/* 小さめスマホ */
@media (max-width: 480px) {
}

</style>