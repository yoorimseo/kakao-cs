<template>
  <Navi/>
  <div class="main">
    <SNB/>
    <Contents/>
  </div>
</template>

<script>
import Navi from './Navi.vue';
import SNB from './SNB.vue';
import Contents from './Contents.vue';

export default {
  name: 'Main',
  components: {
    SNB,
    Contents,
    Navi,
  },
  data() {
    return {
    };
  },
};
</script>

<style scoped>
.main {
  width: 990px;
  min-height: 484px;
  margin: 0 auto;
  display: flex;
  flex-direction: row;
}
</style>
