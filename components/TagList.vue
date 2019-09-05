<template>
  <div>
    <ul class="tag">
      <li v-for="tag in tags" :key="tag" class="tag__item">
        <nuxt-link class="tag__link" :to="`/hashtags/${tag}`">#{{ tag }}</nuxt-link>
      </li>
      <li class="tag__item">
        <nuxt-link class="tag__link" to="/">view all tags</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    tags: {
      type: Array,
      default: () => [
        'morning',
        'meow'
      ]
    }
  }
}
</script>
