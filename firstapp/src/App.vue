<template>
  <div>
    <input type="text" v-model="inputText" placeholder="Metin girin">
    <Text :msg="inputText" />
  </div>
</template>

<script>
import Text from './components/Text.vue'

export default {
  components: {
    Text,
  },
  data() {
    return {
      inputText: ''
    }
  }
}
</script>
