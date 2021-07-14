<template>
  <Navi :naviPath="selectedCategoryName"/>
  <div class="main">
    <SNB
      :categoryNameList="categoryNameList"
      :changeCategory="changeCategory"
      :selectedCategoryName="selectedCategoryName"
    />
    <Contents :questionList="selectedQuestionList" :naviTitle="selectedCategoryName"/>
  </div>
</template>

<script>
import Navi from './Navi.vue';
import SNB from './SNB.vue';
import Contents from './Contents.vue';
import data from '../data/data';

export default {
  name: 'Main',
  components: {
    SNB,
    Contents,
    Navi,
  },
  data() {
    return {
      selectedCategoryName: '일반',
      categoryNameList: ['일반', '인증서', '서비스 이용', 'MY 비밀번호', '디지털 ID', '지갑 QR'],
      selectedQuestionList: data['일반'],
    };
  },
  methods: {
    changeCategory(categoryName) {
      this.selectedCategoryName = categoryName;
      this.selectedQuestionList = data[categoryName];
    },
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
