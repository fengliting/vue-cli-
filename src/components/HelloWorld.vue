<template lang="html">
  <div>
    <editor-bar v-model="editor.info" :isClear="isClear" @change="change"></editor-bar>
  </div>
</template>

<script>

import EditorBar from '@/components/EditorBar'
export default {
  data () {
    return {
      editor: {
        info: ''
      },
      isClear: false
    }
  },
  methods: {
    change (val) {
      this.editor.info1 = val
    }
  },
  components: {
    EditorBar
  }
}
</script>