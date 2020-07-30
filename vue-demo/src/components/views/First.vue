<template>
  <div class="main">
    main part
    <confirm text="注册" @message="getMessage"></confirm>
  </div>
</template>

<script>
import Confirm from '../sub/Confirm'
export default {
  name: 'First',
  components: {
    Confirm
  },
  data () {
    return {
      msg: 'Welcome to FirstApp',
      isCollapse: true
    }
  },
  methods: {
    getMessage (val) {
      alert(val)
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
