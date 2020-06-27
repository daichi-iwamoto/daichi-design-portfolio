<template>
  <section id="section02">
    <div class="section02_box">
      <swiper class="section02_box-swiper" :options="swiperOption">
        <swiper-slide class="section2_box-swiperImg">
          vueのプラグイン「vue-awesome-swiper」を使用したスライドです。
          <br>ナビゲーションボタンのデザイン・アニメーションはSCCで自作しました。
        </swiper-slide>
        <swiper-slide class="section2_box-swiperImg">
          vueのプラグイン「vue-awesome-swiper」を使用したスライドです。
          <br>ナビゲーションボタンのデザイン・アニメーションはSCCで自作しました。
        </swiper-slide>
        <swiper-slide class="section2_box-swiperImg">
          vueのプラグイン「vue-awesome-swiper」を使用したスライドです。
          <br>ナビゲーションボタンのデザイン・アニメーションはSCCで自作しました。
        </swiper-slide>
        <swiper-slide class="section2_box-swiperImg">
          vueのプラグイン「vue-awesome-swiper」を使用したスライドです。
          <br>ナビゲーションボタンのデザイン・アニメーションはSCCで自作しました。
        </swiper-slide>
        <swiper-slide class="section2_box-swiperImg">
          vueのプラグイン「vue-awesome-swiper」を使用したスライドです。
          <br>ナビゲーションボタンのデザイン・アニメーションはSCCで自作しました。
        </swiper-slide>
        <div slot="pagination" class="section02_box-swiperPagination swiper-pagination-bullets" />
      </swiper>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      swiperOption: {
        autoplay: {
          delay: 3000,
          disableOnInteraction: false
        },
        pagination: {
          el: '.section02_box-swiperPagination',
          clickable: true,
          renderBullet (index, className) {
            return `<span class="${className} swiper-pagination-bullet-custom"></span>`
          }
        }
      }
    }
  }
}
</script>
