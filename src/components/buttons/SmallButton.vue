<script setup>
/*import { defineProps } from 'vue'

 const props = defineProps({
  path: {
    type: String,
    required: true
  }
})

後ほどパスを設定する
一旦ホームに戻るようにしてる
*/
</script>

<template>
  <RouterLink to="/" class="btn btn--small">SmallButton</RouterLink>
</template>

<style lang="scss" scoped>
.btn--small {
  width: 45%;
  font-size: 1rem;
  @include btn-secondary;
}
</style>
