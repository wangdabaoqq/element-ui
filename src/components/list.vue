<template>
  <div>
    <!-- <RadioGroup size="small" v-model="radio" @change="changes">
      <Radio border :label="3">111</Radio>
      <Radio border  :label="4">22</Radio>
    </RadioGroup> -->
    <!-- <Row :gutter="20" type="flex" justify="end">
      <Cols :span="6">2</Cols>
      <Cols :span="6">2</Cols>
      <Cols :span="6">2</Cols>
      <Cols :span="6">2</Cols>
    </Row> -->
    <!-- <checkboxGroup v-model="radio"  :min="1" :max="2"> -->
    <!-- <checkbox label="选中且禁用" :indeterminate="true" checked true-label="222" size="small" border v-model="radios" @change="changes">备选项e1</checkbox>
    <checkbox label="123" disabled>备选项2</checkbox>
    <checkbox label="2333">备选项3</checkbox>
    <checkbox label="11">备选项4</checkbox> -->
    <!-- </checkboxGroup> -->
    <!-- <checkboxBut>111</checkboxBut> -->
    <InputNumber v-model="text" :min="1" :max="10"  />
    <!-- <Input v-model="text" size="small" suffix-icon="el-icon-date"  :autosize="{ minRows: 1, maxRows: 4}" clearable type="textarea"  /> -->
  </div>
</template>

<script>
// import Row from 'element-ui/packages/row'
// import Cols from 'element-ui/packages/col'
//  import Radio from 'element-ui/packages/radio'
//  import RadioGroup from 'element-ui/packages/radio-group'
//  import checkbox from 'element-ui/packages/checkbox'
//  import checkboxBut from 'element-ui/packages/checkbox-button'
 import InputNumber from 'element-ui/packages/input-number'

//  import checkboxGroup from 'element-ui/packages/checkbox-group'

 import 'element-ui/lib/theme-chalk/index.css';

export default {
  data () {
    return {
      radio: ['选中且禁用','123'],
      radios: false,
      text: 1
    }
  },
  methods: {
     changes () {
      console.log('radios')
    }
  },
  components: {
    // tree: resolve => require(["./components/ztree.vue"], resolve),
    // setList: () => import ('./setList'),
    // Row,
    // Cols
    // Icon
    // Links
    // Radio,
    // RadioGroup
    // checkbox,
    // checkboxBut
    // Input
    InputNumber
    // checkboxGroup
  },
}
</script>

<style>

</style>