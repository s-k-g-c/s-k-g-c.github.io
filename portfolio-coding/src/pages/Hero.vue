<template>
      <section class="hero">

        <div class="animated-text">
          <span>
            <p>丁寧な構造で、</p>
            <p>意図したレイアウトを</p>
            <p>正確に再現します。</p>
          </span>
        </div>
        </section>
</template>

<style>

.hero {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Yu Gothic', 'Noto Sans JP', sans-serif;
  position: relative;
  overflow: hidden; /* 背景がはみ出ないように */
  min-height: 200px;
  margin: 80px 0 0 0 ;
}

.animated-text {
  font-weight: bold;
  background: linear-gradient(270deg, cyan, magenta, yellow, cyan);
  background-size: 300% 300%;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: gradientShift 15s ease infinite;
  display: inline-block;
  line-height: 1.5;

}

.animated-text span{
  font-size: 2rem;
}


.animated-text p:nth-child(1) { margin-left: 0px; }
.animated-text p:nth-child(2) { margin-left: 30px; }
.animated-text p:nth-child(3) { margin-left: 127px; }



@keyframes gradientShift {
  0% {
    background-position: 0% 50%;
  }
  100% {
    background-position: 100% 50%;
  }
}

/* フェードインと上下動のアニメはJSで文字を一文字ずつ囲んで実装する形がおすすめですが */
/* ここではホバーの揺れのみCSSで例示 */

.animated-text:hover {
  animation: gradientShift 15s ease infinite, swing 0.5s ease infinite;
}

@keyframes swing {
  0%, 100% {
    transform: translateX(0);
  }
  50% {
    transform: translateX(5px);
  }
}

/* タブレット → スマホ（必須） */
@media (max-width: 768px) {
  .animated-text span{
  font-size: 1.8rem;
  }
.animated-text p:nth-child(1) { margin-left: 0px; }
.animated-text p:nth-child(2) { margin-left: 25px; }
.animated-text p:nth-child(3) { margin-left: 97px; }

}

/* 小さめスマホ */
@media (max-width: 480px) {
.animated-text span{
  font-size: 1.6rem;
}
.animated-text p:nth-child(1) { margin-left: 0px; }
.animated-text p:nth-child(2) { margin-left: 20px; }
.animated-text p:nth-child(3) { margin-left: 83px; }
}
</style>