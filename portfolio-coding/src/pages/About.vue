<template>
    <section class="about-text" id="about-text">
        <p>PMO案件の経験を経て、</p>
        <p><span class="keyword cyan">フロントエンド</span>を学習中です。</p>
        <p><span class="keyword green">HTML/CSS</span> を中心に、<p>
        </p>デザインから実装まで一貫して制作しています。</p>
    </section>
</template>

<style>

.about-text {
  padding: 20px 20px;
  width: 415px;
  margin:20px auto 30px;
  font-size: 1.2rem; /* 少し大きめ */
  line-height: 1.6;
  font-family: 'Yu Gothic', 'Noto Sans JP', sans-serif;
  color: #222;
  letter-spacing: 3px;
}

.keyword {
  font-weight: 700;
  font-size: 1.4rem; /* 少し大きめ */
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: gradientFlow 10s linear infinite;
  cursor: pointer;
  display: inline-block;
  transition: transform 0.3s ease;
}

.keyword.turquois-blue {
  background-image: linear-gradient(270deg, #00b87a, #007c53);
}

.keyword.green {
  background-image: linear-gradient(270deg, #00b87a, #007c53);
}

.keyword.cyan {
  background-image: linear-gradient(270deg, #00ffff, #00cccc);
}

.keyword.magenta {
  background-image: linear-gradient(270deg, #ff00ff, #cc00cc);
}

.keyword.yellow {
  background-image: linear-gradient(270deg, #ffcc00, #cc9900);
}

.keyword:hover {
  transform: translateX(5px) rotate(3deg);
}

@keyframes gradientFlow {
  0% {
    background-position: 0% 50%;
  }
  100% {
    background-position: 100% 50%;
  }
}

@media (max-width: 768px) {
  .about-text {
    font-size: 1rem;
    line-height: 1;
    line-height: 1.6;
  }
  .keyword {
  font-size: 1.2rem;
  }
}

/* タブレット → スマホ（必須） */
@media (max-width: 768px) {
.about-text {
  padding: 20px 20px;
  width: 415px;
  margin:20px auto 30px;
  font-size: 1.1rem; /* 少し大きめ */
  line-height: 1.5;
  letter-spacing: 2px;
}
}

/* 小さめスマホ */
@media (max-width: 480px) {

.about-text {
  padding: 20px 0;
  width: 100%;
  margin:20px auto 30px;
  font-size: 1rem;
  line-height: 1.5;
  letter-spacing: 0;
}
}
</style>