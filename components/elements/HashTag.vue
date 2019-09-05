<template>
  <nuxt-link
    :to="`/hashtag/${text}`"
    class="tag"
    :class="block ? 'tag--block' : 'tag--inline'">
    #{{ text }}
  </nuxt-link>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: 'undefined'
    },
    block: {
      type: Boolean,
      default: false
    }
  }
}
</script>
