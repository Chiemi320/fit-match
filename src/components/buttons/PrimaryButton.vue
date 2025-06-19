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
  <RouterLink to="/" class="btn btn--primary">PrimaryButton</RouterLink>
</template>

<style lang="scss" scoped>
.btn--primary {
  width: 100%;
  font-size: 1.2rem;
  @include btn-primary;
}
</style>
