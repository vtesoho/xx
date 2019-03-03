<template>
  <div id="app">
    <img src="./assets/logo.png">
    {{ls.a}}{{ls.b}}
    <div @click="editLs">xx</div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      ls: {
        a: 'a'
      }
    }
  },
  mounted () {
    this.$set(this.ls, 'b', 0)
  },
  methods: {
    editLs: function () {
      this.ls.a = 'aaa'
      this.ls.d = 'ddd'
    }
  }

}
</script>
