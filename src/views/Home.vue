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
  created() {
    console.log('created')
  },
   mounted() {
    console.log('mounted')
  },

  beforeUpdate() {
    console.log('beforUpdated')
  },

  updated() {
    console.log('updated')

  },

  beforeDestroy() {
    console.log('beforeDestroy')

  },

}
</script>