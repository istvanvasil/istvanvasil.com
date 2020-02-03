<template>
  <div
    :style="cursorPoint"
    :class="['dot-cursor', { 'dot-cursor-hide': hideCursor }]"
  ></div>
</template>

<script>
export default {
  name: 'DotCursor',

  data() {
    return {
      xChild: 0,
      yChild: 0,
      xParent: 0,
      yParent: 0,
      hideCursor: true,
      isTouch: false
    }
  },

  computed: {
    cursorPoint() {
      return `transform: translateX(${this.xChild - 3}px) translateY(${this
        .yChild - 3}px) translateZ(0) translate3d(0, 0, 0);`
    }
  },

  mounted() {
    document.addEventListener('mousemove', this.moveCursor)
    document.addEventListener('mouseleave', (e) => {
      this.hideCursor = true
    })
    document.addEventListener('touchstart', (e) => {
      this.isTouch = true
      this.hideCursor = true
    })
    document.addEventListener('mouseenter', (e) => {
      if (this.isTouch) {
        this.hideCursor = true
      } else {
        this.hideCursor = false
      }
    })
  },

  methods: {
    moveCursor(e) {
      this.xChild = e.clientX
      this.yChild = e.clientY
    }
  }
}
</script>

<style>
.dot-cursor-hide {
  opacity: 0;
  transition: opacity 0.15s ease;
}

.dot-cursor {
  top: 0;
  left: 0;
  position: fixed;
  width: 20px;
  height: 20px;
  pointer-events: none;
  user-select: none;
  border-radius: 100%;
  background: var(--off-white);
  z-index: 999999;
  backface-visibility: hidden;
  will-change: transform;
}
</style>
