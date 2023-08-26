<template>
  <div>
    <input type="text" v-model="inputText">
    <Text :msg="inputText" />
    <CalcArea/>
    <Calculator/>
  </div>
</template>

<script>
import Text from './components/Text.vue'
import NumButton from './components/Numbutton.vue'
import CalcArea from './components/CalcArea.vue';
import Calculator from "./components/Calculator.vue";

export default {
  components: {
    Text,
    NumButton,
    CalcArea,
    Calculator
},
  data() {
    return {
      inputText: ''
    }
  }
}
</script>