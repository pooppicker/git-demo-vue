<template>
  <div class="out">
    <label for="account">帳號</label>
    <input @click="alertTest" id="account" type="account" />
  </div>
</template>

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

<style lang="sass" scoped>
input:focus, textarea:focus, select:focus
  outline: none

%input-bottom
  border-bottom: 2px solid #657786
  font-size: 15px
  padding: 0.5em
  &:hover, &:focus
    border-bottom: 2px solid #50B5FF

.out
  @extend %input-bottom
  background-color: #F5F8FA
  width: 400px
  height: 60px
  display: flex
  flex-direction: column
  align-items: start
label
  font-size: 13px
  color: #657786
input
  border: none
  background-color: #F5F8FA
  font-size: 19px

.error-message
  // outline: 1px solid black
  color: #FC5A5A
  display: inline-block
  font-size: 12px
  line-height: 3
  margin: 0
</style>