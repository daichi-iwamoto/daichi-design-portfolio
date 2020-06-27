<template>
  <div class="load">
    <div class="load_wrapper">
      <p class="load_wrapper-txt">
        <span class="load_wrapper-txtSpan">D</span>
        <span class="load_wrapper-txtSpan">e</span>
        <span class="load_wrapper-txtSpan">s</span>
        <span class="load_wrapper-txtSpan">i</span>
        <span class="load_wrapper-txtSpan">g</span>
        <span class="load_wrapper-txtSpan">n</span>
        <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        <span class="load_wrapper-txtSpan">P</span>
        <span class="load_wrapper-txtSpan">o</span>
        <span class="load_wrapper-txtSpan">r</span>
        <span class="load_wrapper-txtSpan">t</span>
        <span class="load_wrapper-txtSpan">f</span>
        <span class="load_wrapper-txtSpan">o</span>
        <span class="load_wrapper-txtSpan">l</span>
        <span class="load_wrapper-txtSpan">i</span>
        <span class="load_wrapper-txtSpan">o</span>
      </p>
    </div>
  </div>
</template>

<script>
import { TweenMax } from 'gsap'

export default {
  mounted () {
    // TweenMax.to('.load_wrapper-txtSpan', 1, { border: '1px solid white', color: 'white' })
    TweenMax.staggerTo('.load_wrapper-txtSpan', 0.5, { delay: 0.3, opacity: '1' }, 0.05)
  }
}
</script>
