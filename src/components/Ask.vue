<template>
    <div class="ask">
        <span class="ask-txt">원하시는 답변을 찾지못하셨다면, 고객센터로 문의해 주세요.</span>
        <div class="ask-btn">
            <img width="17" height="17" class="ask-btn-img" src="https://img.icons8.com/pastel-glyph/2x/pencil--v2.png">
            <span>문의하기</span>
        </div>
    </div>
</template>
<script>
export default {
  name: 'Ask',
};
</script>
<style scoped>
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
