<template>
  <div class="about">
    <h1 @click="alertTest">This is an Home home</h1><HeartFilled />
    
  </div>
</template>

<style lang="scss" scoped>
h1 {
  cursor: pointer;
}
</style>

<script>
import Swal from "sweetalert2";
import HeartFilled from "./../components/logos/HeartFilled.vue"
export default {
  components: {
    HeartFilled
  },
  methods: {
    alertTest() {
      Swal.fire("有成功跳出通知嗎");
    },
  },
};
</script>
