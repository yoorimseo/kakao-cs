<template>
    <div class="list">
        <div class="list-box">
            <div class="list-inner" v-for="(type, num) in questionInfo" v-bind:key="num">
                <span class="list-num">{{num+1}}</span>
                <div class="list-txt">
                    <span>{{type}}</span>
                    <img class="list-btn" src="https://img.pngio.com/down-arrow-icon-png-png-collections-at-251857-png-images-pngio-arrow-down-png-1200_630.png">
                </div>
            </div>
        </div>
        <div class="ask">
            <span class="ask-txt">원하시는 답변을 찾지못하셨다면, 고객센터로 문의해 주세요.</span>
            <div class="ask-btn">
                <img width="17" height="17" class="ask-btn-img" src="https://img.icons8.com/pastel-glyph/2x/pencil--v2.png">
                <span>문의하기</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Question',
  data() {
    return {
      questionInfo: ['카카오 지갑은 어떤 서비스인가요?', '카카오 인증서는 무엇인가요?', '나의 디지털 ID가 무엇인가요?'],
    };
  },
};
</script>

<style scoped>
.list {
  margin: 0;
  padding: 0;
  list-style: none;
  border-top: 2px solid black;
}
.list-box {
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

.ask {
  display: flex;
  justify-content : space-between;
}
.ask-txt {
  display: flex;
  margin-top: 50px;
  font-size: 13px;
  color: #666;
}
.ask-btn {
  width: 186px;
  height: 42px;
  margin: 50px 5px 5px 0;
  background-color: #e8e8e8;
  font-size: 15px;
  font-weight: 600;
  text-align: center;
  cursor: pointer;
}
.ask-btn-img {
  margin: 12px 3px 0 0;
}
</style>
