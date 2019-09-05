<template>
  <component
    :is="btnKind"
    :href="url"
    class="button"
    :class="[
      outline ? 'button--outline' : 'button--primary',
      { 'is-filled': isFilled,
        'button--icon': icon,
        'is-sm': small,
        'is-block': block }]">
    <slot></slot>
  </component>
</template>
<script>
export default {
  props: {
    as: {
      type: String,
      default: 'nuxt-link'
    },
    url: {
      type: String,
      default: '#'
    },
    outline: {
      type: Boolean,
      default: false
    },
    icon: {
      type: Boolean,
      default: false
    },
    filled: {
      type: Boolean,
      default: false
    },
    small: {
      type: Boolean,
      default: false
    },
    block: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    btnKind () {
      switch (this.as) {
        case 'button':
          return 'button'
        case 'link':
          return 'a'
        case 'control':
          return 'input'
      }
    },
    link () {
      if (this.type === 'link') return this.url
    },
    isFilled () {
      if (this.outline) {
        return this.filled
      } else {
        return false
      }
    }
  }
}
</script>
