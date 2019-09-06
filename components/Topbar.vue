<template>
  <div class="main__topbar sticky">
    <span class="main__topbar__title">
      {{ pageTitle }}
    </span>
  </div>
</template>

<script>
export default {
  props: {
    pageTitle: {
      type: String,
      default: 'feed'
    }
  }
}
</script>
