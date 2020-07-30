<template>
  <div class="confirm">
      <el-button @click="getButtonClick">
          {{text || '确认'}}
      </el-button>
  </div>
</template>

<script>
export default {
  name: 'Confirm',
  props: ['text'],
  data () {
    return {
      msg: true
    }
  },
  methods: {
    getButtonClick () {
      this.$emit('message', this.msg)
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
$color: red;
.main {
  color: $color;
}

</style>
