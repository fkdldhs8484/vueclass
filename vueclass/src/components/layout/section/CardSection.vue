<template>
  <section id="cardType" class="card__wrap" :class="attr">
    <span class="blind">카드 유형 01</span>
    <h2>말티즈 강의</h2>
    <p>우리집 말티즈의 귀여움을 알아보자.</p>
    <div class="card__inner" :class="layout">
      <article class="card">
        <figure class="card__header">
          <img src="img/card_bg01_01.jpg" alt="웹표준 사이트 만들기" />
        </figure>
        <div class="card__body">
          <h3 class="tit">말티즈가 한심하게 처다볼때</h3>
          <p class="decs">
            말티즈는 가끔 아니 자주 주인을 한심하게 처다볼때가 많습니다.성격이
            치와와급으로 더럽습니다.자기 마음에 안들면 짖습니다. 간식주면 다
            따라갑니다.
          </p>
          <a class="btn" href="/">
            더 자세히 보기
            <span aria-hidden="true">
              <svg
                width="65"
                height="8"
                viewBox="0 0 65 8"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M64.3536 4.35355C64.5488 4.15829 64.5488 3.84171 64.3536 3.64645L61.1716 0.464466C60.9763 0.269203 60.6597 0.269203 60.4645 0.464466C60.2692 0.659728 60.2692 0.97631 60.4645 1.17157L63.2929 4L60.4645 6.82843C60.2692 7.02369 60.2692 7.34027 60.4645 7.53553C60.6597 7.7308 60.9763 7.7308 61.1716 7.53553L64.3536 4.35355ZM0 4.5H64V3.5H0L0 4.5Z"
                  fill="black"
                />
              </svg>
            </span>
          </a>
        </div>
      </article>
      <article class="card">
        <figure class="card__header">
          <img src="img/card_bg01_02.jpg" alt="웹표준 사이트 만들기" />
        </figure>
        <div class="card__body">
          <h3 class="tit">말티즈가 산책할때</h3>
          <p class="decs">
            말티즈는 산책을 아주 좋아합니다. 간식을 들고 가도 산책을 더 좋아해서
            간식을 처다도 안봅니다.주인이 멈춰도 알아서 자기가 갈길을 갑니다.
          </p>
          <a class="btn" href="/">
            더 자세히 보기
            <span aria-hidden="true">
              <svg
                width="65"
                height="8"
                viewBox="0 0 65 8"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M64.3536 4.35355C64.5488 4.15829 64.5488 3.84171 64.3536 3.64645L61.1716 0.464466C60.9763 0.269203 60.6597 0.269203 60.4645 0.464466C60.2692 0.659728 60.2692 0.97631 60.4645 1.17157L63.2929 4L60.4645 6.82843C60.2692 7.02369 60.2692 7.34027 60.4645 7.53553C60.6597 7.7308 60.9763 7.7308 61.1716 7.53553L64.3536 4.35355ZM0 4.5H64V3.5H0L0 4.5Z"
                  fill="black"
                />
              </svg>
            </span>
          </a>
        </div>
      </article>
      <article class="card">
        <figure class="card__header">
          <img src="img/card_bg01_03.jpg" alt="웹표준 사이트 만들기" />
        </figure>
        <div class="card__body">
          <h3 class="tit">말티즈가 간식 달라고 할때</h3>
          <p class="decs">
            말티즈는 간식을 원할 때 주인을 뚫어져라 처다보거나 간식이 있는
            곳으로 가 짖습니다.한개만 주면 더 달라고 쪼릅니다. 안주면 주인
            다리를 발톱으로 박박 긁습니다.
          </p>
          <a class="btn" href="/">
            더 자세히 보기
            <span aria-hidden="true">
              <svg
                width="65"
                height="8"
                viewBox="0 0 65 8"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M64.3536 4.35355C64.5488 4.15829 64.5488 3.84171 64.3536 3.64645L61.1716 0.464466C60.9763 0.269203 60.6597 0.269203 60.4645 0.464466C60.2692 0.659728 60.2692 0.97631 60.4645 1.17157L63.2929 4L60.4645 6.82843C60.2692 7.02369 60.2692 7.34027 60.4645 7.53553C60.6597 7.7308 60.9763 7.7308 61.1716 7.53553L64.3536 4.35355ZM0 4.5H64V3.5H0L0 4.5Z"
                  fill="black"
                />
              </svg>
            </span>
          </a>
        </div>
      </article>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    attr: String,
    layout: String,
  },
};
</script>

<style>
/* cartType */
.card__inner {
  display: flex;
  justify-content: space-between;
}
.card {
  width: 32%;
  background: #f5f5f5;
}
.card__body {
  padding: 24px;
}
.card__body .tit {
  font-size: 24px;
  margin-bottom: 10px;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}
.card__body .desc {
  font-size: 18px;
  line-height: 1.4;
  color: #666;
  margin-bottom: 20px;
  font-weight: 300;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
}

@media (max-width: 960px) {
  .card__inner {
    flex-wrap: wrap;
  }
  .card {
    width: 49%;
  }
  .card:last-child {
    display: none;
  }
}
@media (max-width: 600px) {
  .card {
    width: 100%;
  }
  .card:first-child {
    margin-bottom: 20px;
  }
  .card__body {
    padding: 20px;
  }
  .card__body .desc {
    font-size: 16px;
  }
}
</style>
