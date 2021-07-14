<template>
  <div class="list-question" @click="toggleShow()">
    <span class="list-num">{{num}}</span>
    <div class="list-txt">
      <span :class="{'list-h3': isShow}">{{question.question}}</span>
      <img
        class="list-btn"
        src="https://img.pngio.com/down-arrow-icon-png-png-collections-at-251857-png-images-pngio-arrow-down-png-1200_630.png"
      >
    </div>
  </div>
  <div class="list-answer" v-show="isShow">
    <span>{{question.answer}}</span>
  </div>
</template>

<script>
export default {
  name: 'Question',
  props: ['question', 'num'],
  data() {
    return {
      isShow: false,
    };
  },
  methods: {
    toggleShow() {
      this.isShow = !this.isShow;
      // if (this.isShow) {
      //   this.isShow = false;
      // } else {
      //   this.isShow = true;
      // }
    },
  },
};
</script>

<style scoped>
.list-question {
  display: flex;
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
  cursor: pointer;
}
.list-answer {
  color: #1e1e1e;
  width: 680px;
  margin: 5px;
  margin-left: 60px;
  font-size: 15px;
  cursor: pointer;
}
.list-btn {
  width: 30px;
  height: 16px;
  float: right;
}
.list-h3 {
  font-size: 1.3rem;
  font-weight: bold;
}
</style>
