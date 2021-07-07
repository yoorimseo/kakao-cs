<template>
    <div class="snb">
      <h2 class="snb-title">카카오톡 지갑</h2>
      <ul class="snb-list">
        <li class="snb-list-txt" v-for="name in categoryName" :key="name">{{name}}</li>
      </ul>
    </div>
</template>

<script>
export default {
  name: 'SNB',
  data() {
    return {
      categoryName: ['일반', '인증서', '서비스 이용', 'MY 비밀번호', '디지털 ID', '지갑 QR'],
    };
  },
};
</script>

<style scoped>
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
  color: #878787;
  cursor: pointer;
}
.snb-list-txt:hover {
    text-decoration: 1px black underline;
    color: black;
}
</style>
