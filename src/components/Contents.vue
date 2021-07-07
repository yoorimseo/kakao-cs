<template>
    <div class="contents">
        <h1 class="title">일반</h1>
        <div class="sub-title">
            <a href="#" class="sub-txt">OS 공통</a>
        </div>
        <Question/>
    </div>
</template>

<script>
import Question from './Question.vue';

export default {
  name: 'Contents',
  components: {
    Question,
  },
};
</script>

<style scoped>
.contents {
  height: 700px;
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
</style>
