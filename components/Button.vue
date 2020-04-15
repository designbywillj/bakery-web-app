<template>
  <button
    type="button"
    class="button"
    :class="{ 'button--primary': primary, 'button--secondary': secondary }"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: ''
    },
    primary: {
      type: Boolean
    },
    secondary: {
      type: Boolean
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/_colors.scss';

.button {
  width: 100%;
  height: 3rem;
  border-radius: 1.5rem;
  font-weight: 700;

  &--primary {
    background-color: $color--pink;
    color: $color--white;
  }

  &--secondary {
    background-color: $color--gray;
  }
}
</style>
