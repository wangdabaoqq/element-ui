<template>
  <div id="app" class="flex-col">
   
    <!-- <RadioGroup size="small" @change="changes" v-model="radio">
      <Radio border :label="3">111</Radio>
      <Radio border  :label="4">22</Radio>
    </RadioGroup> -->
    <list />
  </div>
</template>

<script>
//  import Row from 'element-ui/packages/row'
//  import Cols from 'element-ui/packages/col'
//  import Links from 'element-ui/packages/link'
//  import Radio from 'element-ui/packages/radio'
//  import RadioGroup from 'element-ui/packages/radio-group'

//  import 'element-ui/lib/theme-chalk/index.css';


export default {
  name: "app",
  components: {
    list: () => import('./components/list')
    // Row,
    // Cols,
    // Icon
    // Links
    // Radio,
    // RadioGroup
  },
  data() {
    return {
    }
  },
};
</script>

<style>
html,body{height: 100%;}
body {
  margin: 0;
}
/* 自定义按钮样式 */
.tree_extra_btn{
  display: inline-block;
  padding: 0 3px;
  color: red;
}

/* flex栅格 */
.flex-col {
  overflow: hidden;
  display: -ms-box;
  display: -ms-flexbox;
  display: flex;
  flex-direction: column;
  -ms-flex-direction: column;
}

.flex-row {
  overflow: hidden;
  display: -ms-box;
  display: -ms-flexbox;
  display: flex;
}

.flex-1 {
  -ms-flex: 1;
  flex: 1;
  min-width: 0;
}

.flex-2 {
  -ms-flex: 2;
  flex: 2;
  min-width: 0;
}

.flex-3 {
  -ms-flex: 3;
  flex: 3;
  min-width: 0;
}

.flex-4 {
  -ms-flex: 4;
  flex: 4;
  min-width: 0;
}

.align-stretch {
  -ms-align-items: stretch;
  -ms-flex-align: stretch;
  align-items: stretch;
}

.align-center {
  -ms-align-items: center;
  -ms-flex-align: center;
  align-items: center;
}

.justify-center {
  -ms-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
}

#app {
  height: 100%;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.wrap{
  overflow: hidden;
}
.c {
  width: 600px;
  height: 100%;
  overflow: auto;
  margin: auto;
}
/* .T {
  font-size: 34px;
  margin: 0 0 30px;
  height: 170px;
  line-height: 260px;
  overflow: hidden;
  background:url(./assets/logo.png) center no-repeat;
} */
.toolbar {
  margin: 20px auto;
}
.toolbar .btn {
  padding: 0.5em 1em;
  outline: none;
  border-radius: 4px;
}

.foot {
  margin-top: 30px;
  background: #333;
  padding: 24px;
  overflow: hidden;
  color: #999;
  font-size: 14px;
  text-align: center;
}

.foot a {
  color: #fff;
  margin: 0 0.5em;
}
</style>
