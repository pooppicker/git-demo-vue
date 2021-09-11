<template>
  <div class="about">
    <h1 @click="alertTest"> This is an Home home</h1>
  </div>
</template>

<style lang="scss" scoped>
h1 {
  cursor: pointer;
}

</style>

<script>
import Swal from 'sweetalert2'
export default {
  
  methods: {
    alertTest() {
      Swal.fire('有成功跳出通知嗎')
    }

  },
}
</script>