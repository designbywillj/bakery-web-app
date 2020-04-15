<template>
  <div class="input">
    <label class="input__label">{{ label }}</label>
    <input v-if="text" type="text" class="input__text" />
    <input v-if="email" type="email" class="input__text" />
    <textarea v-if="textarea" class="input__textarea" />
  </div>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: ''
    },
    text: {
      type: Boolean
    },
    email: {
      type: Boolean
    },
    textarea: {
      type: Boolean
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/_colors.scss';

.input {
  margin-bottom: 1.5rem;

  &__label {
    display: block;
    line-height: 2rem;
    margin-bottom: 0.5rem;
    font-weight: 700;
  }

  &__text {
    width: 100%;
    height: 3rem;
    padding: 0 0.75rem;
    background-color: $color--gray;
    border-radius: 0.5rem;
  }

  &__textarea {
    @extend .input__text;
    height: 180px;
    padding-top: 0.75rem;
    padding-bottom: 0.75rem;
    resize: none;
  }
}
</style>
