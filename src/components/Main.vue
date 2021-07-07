<template>
  <div class="main">
    <div class="snb">
      <h2 class="snb-title">카카오톡 지갑</h2>
      <ul class="snb-list">
        <li class="snb-list-txt">일반</li>
        <li class="snb-list-txt">인증서</li>
        <li class="snb-list-txt">서비스 이용</li>
        <li class="snb-list-txt">MY 비밀번호</li>
        <li class="snb-list-txt">디지털 ID</li>
        <li class="snb-list-txt">지갑 QR</li>
      </ul>
    </div>
    <div class="contents">
      <h1 class="contents-title">일반</h1>
      <div class="contents-sub-title">
        <span class="contents-sub-txt">OS 공통</span>
      </div>
      <div class="contents-list">
        <div class="contents-list-box">
          <div class="contents-list-inner">
            <span class="contents-list-num">1</span>
            <div class="contents-list-txt">카카오톡 지갑은 어떤 서비스인가요?</div>
            <img class="content-list-btn" src="https://img.pngio.com/down-arrow-icon-png-png-collections-at-251857-png-images-pngio-arrow-down-png-1200_630.png">
          </div>
          <div class="contents-list-inner">
            <span class="contents-list-num">2</span>
            <div class="contents-list-txt">카카오 인증서는 무엇인가요?</div>
          </div>
          <div class="contents-list-inner">
            <span class="contents-list-num">3</span>
            <div class="contents-list-txt">나의 디지털 ID가 무엇인가요?</div>
          </div>
        </div>
        <div class="contents-ask">
          <span class="contents-ask-txt">원하시는 답변을 찾지못하셨다면, 고객센터로 문의해 주세요.</span>
          <div class="contents-ask-btn">
            <img class="contents-ask-btn-img" src="https://img.icons8.com/pastel-glyph/2x/pencil--v2.png">
            <span>문의하기</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Main',
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

.snb {
  width: 160px;
  padding-right: 20px;
  float: left;
}
.snb-title {
  font-size: 21px;
  margin-top: 50px;
}
.snb-list {
  margin: 50px 0 0 0;
  padding: 0;
  list-style: none;
}
.snb-list-txt {
  font-size: 15px;
  font-weight: 600;
  margin: 0 0 20px 5px;
}

.contents {
  height: 700px;
  padding: 0 0 60px 58px;
  border-left: 1px solid #e8e8e8;
}
.contents-title {
  width: 750px;
  margin: 47px 0 45px 0;
}

.contents-sub-title {
  height: 37.4px;
  margin-top: 26px;
  padding: 17px 5px 4px;
  border-top: 2px solid black;
}
.contents-sub-txt {
  padding: 5px 0 5px;
  margin: 5px 0 1px 5px;
  font-size: 15px;
  font-weight: 600;
  text-decoration-line: underline;
}

.contents-list {
  margin: 0;
  padding: 0 0 30px 0;
  list-style: none;
  border-top: 2px solid black;
  border-bottom: 1px solid black;
}
.contents-list-box {
  margin-top: 30px;
  padding-bottom: 30px;
  border-bottom: 1px solid black;
}
.contents-list-inner {
  display: flex;
  flex-direction: row;
  padding: 12px 0 16px 0;
  border-bottom: 1px solid #e8e8e8;
}
.contents-list-num {
  width: 55px;
  margin: 5px 0 0 5px;
  color: #1e1e1e;
  border: 1px solid blue;
  font-size: 15px;
}
.contents-list-txt {
  color: #1e1e1e;
  margin: 5px;
  border: 1px solid blue;
  font-size: 15px;
}
.content-list-btn {
  width: 26px;
  height: 12px;
  margin: 5px;
  border: 1px solid blue;
}

.contents-ask {
  height: 97px;
  border: 1px solid green;
  display: flex;
  flex-direction: row;
}
.contents-ask-txt {
  margin-top: 50px;
  font-size: 13px;
  color: #666;
}
.contents-ask-btn {
  width: 186px;
  height: 42px;
  margin: 50px 5px 5px 0;
  background-color: #e8e8e8;
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
}
.contents-ask-btn-img {
  width: 17px;
  height: 17px;
  margin: 12px 3px 0 0;
}
</style>
