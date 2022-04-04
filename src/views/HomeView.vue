<template>
  <p v-html="t('message')"></p>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

// https://velog.io/@latte_h/Vue3-Guide-17-Vue-3%EC%97%90%EC%84%9C-%EB%8B%A4%EA%B5%AD%EC%96%B4-%EC%B2%98%EB%A6%AC
// Components
import { useI18n } from 'vue-i18n'

export default defineComponent({
  name: 'HomeView',

  components: {
  },
  setup() {
    const { t } = useI18n({
      inheritLocale: true,
      useScope: 'local'
    })

    // Something todo ..

    return { t }
  }
});
</script>
