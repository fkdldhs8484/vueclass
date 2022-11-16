<template>
  <section id="imageType" class="image__wrap" :class="attr">
    <span class="blind">이미지 유형01</span>
    <h2>레서판다</h2>
    <p>레서판다의 귀여움을 알아보자.</p>
    <div class="image__inner" :class="layout">
      <article class="image img1">
        <h3 class="image__tit">레서판다가 줄 타는 모습</h3>
        <p class="image__desc">
          레서판다가 줄타는 모습을 보십시오. 너무 귀엽지 않나요.. 귀여워서
          깨물고 <br />
          싶어요...너구리랑 햇갈리지 맙시다.
        </p>
        <a class="image__btn" href="/" title="자세히보기">자세히보기</a>
      </article>
      <article class="image img2">
        <h3 class="image__tit">레서판다의 귀여운 모습</h3>
        <p class="image__desc">
          가만히 있어도 귀여운 헤서판다. 래교부리는 모습도 너무 귀엽다. 너구리랑
          햇갈리지 맙시다..
        </p>
        <a class="image__btn yellow" href="/" title="자세히보기">자세히보기</a>
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
/* image */
.image__wrap {
}
.image__inner {
  display: flex;
  justify-content: space-between;
}

.image {
  width: 48%;
  height: 370px;
  padding: 200px 20px 20px 20px;
  box-sizing: border-box;
  color: #fff;
}
.image.img1 {
  background: url(/src/assets/img/imgType01_1.jpg) no-repeat center / cover;
}
.image.img2 {
  background: url(/src/assets/img/imgType01_2.jpg) no-repeat center / cover;
}
.image__tit {
  font-size: 32px;
  margin-bottom: 10px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

.image__desc {
  font-size: 16px;
  margin-bottom: 10px;
  line-height: 1.4;
  font-weight: 300;
  padding-right: 100px;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}

.image__btn {
  font-size: 16px;
  font-weight: 300;
  color: #fff;
  background: #ba5a30;
  padding: 10px 20px;
  display: inline-block;
}
.image__btn.yellow {
  background-color: #b59140;
}

@media (max-width: 960px) {
}

@media (max-width: 600px) {
  .image__inner {
    flex-direction: column; /*사진을 밑으로 보내줌*/
  }
  .image {
    width: 100%;
    padding: 210px 20px 30px 30px;
  }
  .image:first-child {
    margin-bottom: 20px;
  }
  .image__title {
    font-size: 24px;
  }
}
</style>
