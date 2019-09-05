<template>
  <div>
    <div style="width: 279px; margin-bottom: 20px;">
      <HashTag
        v-for="(tag, index) in tags"
        :key="index"
        :text="tag"
        block/>
    </div>
    <div style="margin-bottom: 20px;">
      <HashTag
        v-for="(tag, index) in tags"
        :key="index"
        :text="tag" />
    </div>
    <div style="margin-bottom: 20px;">
      <CcButton
        as="link"
        href="#">
        link
      </CcButton>
      <CcButton
        type="submit">
        submit btn
      </CcButton>
      <CcButton
        as="control"
        type="submit"
        value="submit input"/>
      <CcButton
        as="control"
        type="reset"
        value="reset input"/>
      <CcButton
        as="control"
        type="button"
        value="btn input"/>
    </div>
    <div style="margin-bottom: 20px">
      <CcButton
        as="link"
        href="#"
        outline>
        link
      </CcButton>
      <CcButton
        type="submit"
        outline>
        submit btn
      </CcButton>
      <CcButton
        type="submit"
        outline
        icon>
        <svg fill="currentColor" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M5 10a5 5 0 1 1 3.95-1.934l3.367 3.367-.884.884L8.066 8.95A4.978 4.978 0 0 1 5 10zm3.75-5a3.75 3.75 0 1 1-7.5 0 3.75 3.75 0 0 1 7.5 0z"/></svg>
      </CcButton>
    </div>
    <div style="margin-bottom: 20px;">
      <CcButton
        outline
        small>
        {{ isSaved ? 'saved' : 'save' }}
      </CcButton>
      <CcButton
        small>
        {{ isSaved ? 'saved' : 'save' }}
      </CcButton>
    </div>
  </div>
</template>
<script>
import HashTag from '@/components/elements/HashTag'
import CcButton from '@/components/elements/CcButton'
export default {
  components: {
    HashTag,
    CcButton
  },
  data () {
    return {
      tags: ['meow', 'purrfect', 'bathing'],
      isSaved: false
    }
  }
}
</script>
