<template>
  <aside class="sidebar">
    <SearchBar />
    <div class="sidebar__content">
      <TagList />
      <CcButton
        as="link"
        url="/create"
        block>new concat
      </CcButton>
    </div>
  </aside>
</template>

<script>
import SearchBar from '@/components/SearchBar'
import TagList from '@/components/TagList'
import CcButton from '@/components/elements/CcButton'

export default {
  components: {
    SearchBar,
    TagList,
    CcButton
  }
}
</script>
