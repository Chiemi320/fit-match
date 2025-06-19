<script setup>
import { defineProps, computed } from 'vue'

const props = defineProps({
  to: {
    type: [String, Object],
    required: true,
  },
  variant: {
    type: String,
    default: 'default',
    validator: (value) => ['default', 'login', 'signup', 'small'].includes(value),
  },
  external: {
    type: Boolean,
    default: false,
  },
  disabled: {
    type: Boolean,
    default: false,
  },
})

console.log('header', props)

const linkClasses = computed(() => {
  return ['link', `link--${props.variant}`, { 'link--disabled': props.disabled }]
})
</script>

<template>
  <RouterLink
    :to="to"
    :class="linkClasses"
    :target="external ? '_blank' : undefined"
    :rel="external ? 'noopener noreferrer' : undefined"
  >
    <slot />
  </RouterLink>
</template>

<style lang="scss" scoped>
.link {
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 2rem;
}

.link--login {
  width: 5.5rem;
  height: var(--link-size-l);
  border: 1px solid var(--link-color-primary);
  background-color: var(--link-color-secondary);
}

.link--signup {
  width: 5.5rem;
  height: var(--link-size-l);
  color: var(--text-white);
  background-color: var(--link-color-primary);
}

.link--small {
  width: 12rem;
  height: var(--link-size-l);
  border: 1px solid var(--link-color-primary);
  background-color: var(--link-color-secondary);
}
</style>
