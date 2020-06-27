<template>
  <section v-scroll="handleScroll" class="section01_box">
    <div class="section01_box-card">
      <div class="section01_box-cardImg">
        <div class="section01_box-cardImgDummy" />
        <p class="section01_box-cardImgTxt">
          dummy img
        </p>
      </div>
      <div class="section01_box-cardDesc">
        <p class="section01_box-cardDescTxt">
          vueのカスタムディレクティブで作成した
          <br>該当箇所まで来たらフェードインするアニメーションです。
          <br>グラデーションのアニメーションはCSSで作成して
          <br>画像の代替で置いています。
          <br>
          <br>ヘッダー・フッダーにあるページ内リンクは
          <br>「vue-scrollto.js」を使用しています。
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    handleScroll (evt, el) {
      const rect = el.getBoundingClientRect()
      if (window.scrollY + 30 > rect.top) {
        el.setAttribute(
          'style',
          'opacity: 1;'
        )
      }
      return window.scrollY + 30 > rect.top
    }
  }
}
</script>
