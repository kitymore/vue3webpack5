<template>
  <div>
    
    <h3>Graduated from South China Agricultural University</h3>
    <h3>Expert in javascript react vue weapp and so on!</h3>
    <h3>The following are the details:</h3>
   
    <p>You have stay here for {{ count }} seconds!</p>
  </div>
</template>
<script lang="ts">
import { defineComponent, computed } from 'vue'
import { useStore } from 'vuex'

export default defineComponent({
  name: 'AboutMe',
  setup() {
    const store = useStore()
    const count = computed(() => store.state.count)
    return { count }
  },
})
</script>
<style scoped lang="less">
a {
  color: #42b983;
}

.link a {
  display: inline-block;
  margin: 0 20px;
}
</style>
