<template>
 <div class="page">
 <SplitPane 
  direction="column" 
  :min="20" 
  :max="80" 
  :triggerLength="20" 
  :paneLengthPercent.sync="paneLengthPercent" 
 >
  <template v-slot:one>
  <div>
   区域一
  </div>
  </template>

  <template v-slot:two>
  <div>
   区域二
  </div>
  </template>

 </SplitPane>
 </div>
</template>

<script>
import SplitPane from './components/split-pane'

export default {
 components: {
 SplitPane
 },
 data() {
 return {
  paneLengthPercent: 30
 }
 }
}
</script>

<style scoped lang="scss">
.page {
 height: 100%;
 padding: 10px;
 background: #000;
}
</style>

