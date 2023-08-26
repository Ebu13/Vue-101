<template>
  <div>
    <input type="text" v-model="inputText">
    <Text :msg="inputText" />
    <CalcArea/>
  </div>
</template>

<script>
import Text from './components/Text.vue'
import NumButton from './components/NumButton.vue'
import CalcArea from './components/CalcArea.vue';

export default {
  components: {
    Text,
    NumButton,
    CalcArea
},
  data() {
    return {
      inputText: ''
    }
  }
}
</script>
