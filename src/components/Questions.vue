<template>
    <div class="list-box">
        <div class="list">
            <div class="list-inner" v-for="(type, num) in questionInfo" :key="num">
                <span class="list-num">{{num+1}}</span>
                <div class="list-txt">
                    <span>{{type}}</span>
                    <img class="list-btn" src="https://img.pngio.com/down-arrow-icon-png-png-collections-at-251857-png-images-pngio-arrow-down-png-1200_630.png">
                </div>
            </div>
        </div>
        <Ask/>
    </div>
</template>

<script>
import Ask from './Ask.vue';

export default {
  name: 'Question',
  components: {
    Ask,
  },
  data() {
    return {
      questionInfo: ['카카오톡 지갑은 어떤 서비스인가요?', '카카오 인증서는 무엇인가요?', '나의 디지털 ID가 무엇인가요?'],
    };
  },
};
</script>

<style scoped>
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
  padding: 12px 0 16px 0;
  border-bottom: 1px solid #e8e8e8;
}
.list-num {
  width: 55px;
  margin: 5px 0 0 5px;
  color: #1e1e1e;
  font-size: 15px;
}
.list-txt {
  color: #1e1e1e;
  width: 680px;
  margin: 5px;
  font-size: 15px;
  cursor: pointer;
}
.list-btn {
  width: 30px;
  height: 16px;
  float: right;
}
</style>
