<template>
<section class="works-list" id="works-list">
  <div class="work-item">
    <h3 class="title"><span>ポートフォリオサイト</span><span><small>※このサイトです。</small></span></h3>
    <div class="desc">
      <p><strong>制作月　：</strong>2025年6月</p>
      <p><strong>画面数　：</strong>1</p>
      <p><strong>制作期間：</strong>約3日</p>
      <p><strong>使用技術：</strong>HTML、CSS、JavaScript、Vue</p>
      <p><strong>担当：</strong>デザイン / コーディング</p>
      <p><strong>機能実装：</strong><br>レスポンシブ、Vueコンポーネントなど</p>
    </div>
    <div class="site-seeing">
      <a
        href="https://s-k-g-c.github.io/portfolio-coding/"
        target="_blank"
        rel="noopener noreferrer"
        class="visit-link"
      >
        サイトを見る
      </a>
    </div>

    <div class="work-video">
      <a href="https://s-k-g-c.github.io/portfolio-coding/" target="_blank" rel="noopener noreferrer">
        <img src="/src/assets/port-folio-site.png" alt="ポートフォリオサイト" />
      </a>
    </div>

    <div class="detail">
      <p><strong>概要：</strong></p>
      <p>ポートフォリオ公開を目的に、デザインから実装まで制作。</p>
      <p>背景アニメーションやホバー演出など、画面全体に動きを取り入れつつ、見やすさとのバランスを意識して構築しました。
      </p>
      <p>以降の作品含め、公開には GitHub Pages を使用し、設定やエラー対応まで一通り経験しています。</p>
    </div>
  </div>

  <div class="work-item">
    <h3 class="title"><span>架空コーポレートサイト</span><span></span></h3>
    <div class="desc">
      <p><strong>制作月　：</strong>2025年12月</p>
      <p><strong>画面数　：</strong>6</p>
      <p><strong>制作期間：</strong>5日</p>
      <p><strong>使用技術：</strong>HTML / CSS / JavaScript / Vue</p>
      <p><strong>担当：</strong>デザイン / コーディング</p>
      <p><strong>機能実装：</strong><br>レスポンシブ対応、ハンバーガーメニュー</p>
    </div>

    <div class="site-seeing">
      <a
        href="https://s-k-g-c.github.io/good-sleep-peace/"
        target="_blank"
        rel="noopener noreferrer"
        class="visit-link"
      >
        サイトを見る
      </a>
    </div>

    <div class="work-video">
      <a href="https://s-k-g-c.github.io/good-sleep-peace/" target="_blank" rel="noopener noreferrer">
        <img src="/src/assets/Motion-Palette.png" alt="架空コーポレートサイト" />
      </a>
    </div>

    <div class="detail">
      <p><strong>概要：</strong></p>
      <p>架空の企業を想定し、トップページのデザインと実装を行った制作物。</p>
      <p>企業サイトらしい落ち着いた配色と情報整理を意識し、見やすいレイアウトになるよう構成しました。</p>
      <p>セクションごとの余白調整や階層構造を丁寧に作り、レスポンシブ対応も実装しています。</p>
      <p>HTML / CSS を中心に、コーポレートサイトの基本的なUI構成を学ぶ目的で制作しました。</p>
    </div>
  </div>

  <div class="work-item">
    <h3 class="title"><span>CSSアニメーションの</span><span>サンプルサイト</span></h3>
    <div class="desc">
      <p><strong>制作月　：</strong>2025年6月</p>
      <p><strong>画面数　：</strong>1</p>
      <p><strong>制作期間：</strong>約3日</p>
      <p><strong>使用技術：</strong>HTML / CSS / JavaScript / Vue</p>
      <p><strong>担当：</strong>デザイン / コーディング</p>
      <p><strong>機能実装：</strong><br>Vueコンポーネント、キーフレームアニメーションなど</p>
    </div>

    <div class="site-seeing">
      <a
        href="https://s-k-g-c.github.io/Motion-Palette/"
        target="_blank"
        rel="noopener noreferrer"
        class="visit-link"
      >
        サイトを見る
      </a>
    </div>

    <div class="work-video">
      <a href="https://s-k-g-c.github.io/Motion-Palette/" target="_blank" rel="noopener noreferrer">
        <img src="/src/assets/Motion-Palette.png" alt="CSSアニメーションサンプルサイト" />
      </a>
    </div>

    <div class="detail">
      <p><strong>概要：</strong></p>
      <p>CSSアニメーションの学習を目的に制作。</p>
      <p>四角いオブジェクトの動きはキーフレームで自然なループになるよう調整しました。</p>
      <p>2画面構成ですが、Vueでコンポーネント分割を行い、サイズに応じたレスポンシブ表示を実装。</p>
      <p>全体のデザインはグラデーションを使い、色数を抑えて統一感を持たせています。</p>
    </div>
  </div>

</section>
</template>

<style>

.site-seeing{
  grid-area: link;
  padding: 0.5rem;
  line-height: 1.5;  
  border-radius: 8px;
  display: flex;
}

.site-seeing .visit-link {
  margin-left: auto;
  display: inline-block;
  font-size: 1rem;
  font-weight: 500;
  color: #007ACC; /* 落ち着いた青系、Vueのイメージにも合う */
  text-decoration: none;
  position: relative;
  transition: color 0.2s ease;
}

.work-item:nth-of-type(even) .visit-link {
  margin-left: 0;
  margin-right: auto;
}

.visit-link::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -2px;
  width: 100%;
  height: 1px;
  background: #007ACC;
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.3s ease;
}

.visit-link:hover {
  color: #005f99;
}

.visit-link:hover::after {
  transform: scaleX(1);
}


.works-list {
  gap: 40px;
  padding: 2rem 1rem;
}

.work-item {
  display: grid;
  grid-template-areas:
    "title title"
    "desc video"
    "link video"
    "detail detail";
  grid-template-columns: 1fr 1fr ;
  gap: 20px 40px;
  padding: 2rem;
  border-radius: 12px;
}

.work-item:nth-child(even) {
  display: grid;
  grid-template-areas:
    "title title"
    "video desc"
    "video link"
    "detail detail";
    grid-template-columns: 1fr 1fr;
}

.title {
  grid-area: title;
  font-size: 1.5rem;
  font-weight: 700;
  border-bottom:1px solid gray ;
  
}

.title small{
  font-size: 10px;
}

.desc {
  grid-area: desc;
  border-radius: 8px;
  padding: 0.5rem;
  line-height: 1.5;
}
.work-item{
  justify-content: center; 
  align-items: center;    
  border-radius: 8px;
  padding: 1rem;
}


.work-video {
  grid-area: video;
  width: 100%;             /* 親幅いっぱい（レスポンシブ） */
  aspect-ratio: 16 / 9;    /* ← 16:9比率を維持！ */
  overflow: hidden;
  box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.2);
  border-radius: 8px;
}

.work-video img{
  max-width: 100%;
  display: block; /* ブラウザの余白を抑える */
  width: 100%;
  height: 100%;
  object-fit: cover;  /* これがポイント！ */
  object-position: top; /* 画像の中心を優先して切り取る（任意） */
}

/* .work-video video {
  width: 100%;
  height: auto;
  max-width: 100%;
  border-radius: 8px;
  display: block;
  box-shadow: inset;
  box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.5);
} */

.detail {
  grid-area: detail;
  border-radius: 8px;
  padding: 0.5rem;
  line-height: 1.7;
  font-size: 15px;
  color: #333;
}

@media (max-width: 768px) {
  .works-list {
  gap: 0px;
  padding: 0rem 0rem;
  }

  .work-item{
    grid-template-areas:
      "title"
      "video"
      "link"
      "desc"
      "detail";
    grid-template-columns: 1fr;
  }
  .work-item:nth-child(even) {
    grid-template-areas:
      "title"
      "video"
      "link"
      "desc"
      "detail";
    grid-template-columns: 1fr;
  }

    .work-video {
    width: 100%;
    max-width: 100%;
  }

  .site-seeing{
    justify-content: center;
  }

  .site-seeing .visit-link {
  margin-left: auto;
  margin-right: auto;
}

.work-item:nth-of-type(even) .visit-link {
  margin-left: auto;
  margin-right: auto;
}
  .site-seeing{
  padding: 0.3rem;
  line-height: 1.3;
  margin-top: -5px;
}
}

@media (max-width: 967px) {
  span::after {
    content: "\A";       /* 改行コード */
    white-space: pre;    /* 改行を反映させる */
  }
  .detail p {
  font-size: 15px;
  line-height: 20px; /* 固定の高さにしたい場合 */
}
.site-seeing{
  padding: 0rem;
  line-height: 1.0;
  margin-top: -10px;
}
}

</style>
