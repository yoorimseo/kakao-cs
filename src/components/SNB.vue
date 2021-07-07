<template>
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
</template>

<script>
export default {
  name: 'SNB',
};
</script>

<style>
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
</style>
