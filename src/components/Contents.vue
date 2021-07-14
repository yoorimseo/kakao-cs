<template>
  <div class="contents">
    <h1 class="title">{{naviTitle}}</h1>
    <div class="sub-title">
      <a href="#" class="sub-txt">OS 공통</a>
    </div>
    <div class="list-box">
      <div class="list">
          <div class="list-inner" v-for="(question, num) in questionList" :key="num">
            <Questions :question="question" :num="num+1"/>
          </div>
      </div>
      <Ask/>
    </div>
  </div>
</template>

<script>
import Questions from './Questions.vue';
import Ask from './Ask.vue';

export default {
  name: 'Contents',
  components: {
    Questions,
    Ask,
  },
  props: ['naviTitle', 'questionList'],
};
</script>

<style scoped>
.contents {
  min-height: 700px;
  padding: 0 0 60px 58px;
  border-left: 1px solid #e8e8e8;
}

.title {
  width: 750px;
  margin: 47px 0 45px 0;
}

.sub-title {
  height: 37.4px;
  margin-top: 26px;
  padding: 17px 5px 4px;
  border-top: 2px solid black;
}
.sub-txt {
  padding: 5px 0 5px;
  margin: 5px 0 1px 5px;
  font-size: 15px;
  font-weight: 600;
  text-decoration-line: underline;
  cursor: pointer;
}
.list-box {
  margin: 0;
  padding: 0;
  list-style: none;
  border-top: 2px solid black;
}
.list {
  margin-top: 30px;
  padding-bottom: 30px;
  border-bottom: 1px solid black;
}
.list-inner {
  display: flex;
  flex-direction: column;
  padding: 12px 0 16px 0;
  border-bottom: 1px solid #e8e8e8;
}
</style>
