<template>
    <div class="header">
        <div class="head">
            <Head/>
        <div class="head-inner">
            <a href="https://cs.kakao.com/" class="logo">
            <img src="https://cs.kakao.com/img/cskakaocom/pc/tit_cs2.gif">
            </a>
            <div class="search">
            <input class="search-inner" type="search" placeholder="궁금한 점이 있다면 도움말을 검색해 보세요.">
            <button class="search-btn">
                <img class="search-btn-img" src="https://www.seekpng.com/png/full/871-8719667_download-png-transparent-background-search-icon.png">
            </button>
            </div>
        </div>
        </div>
        <div class="navi">
        <div class="navi-inner">
            <ul class="navi-list">
            <li class="navi-list-txt">
                <a href="#">홈</a>
                <span class="navi-list-arrow">></span>
            </li>
            <li class="navi-list-txt">
                <a href="#">카카오톡 지갑</a>
                <span class="navi-list-arrow">></span>
            </li>
            <li class="navi-list-txt">
                <a href="#">일반</a>
            </li>
            </ul>
        </div>
        </div>
    </div>
</template>

<script>
import Head from './Head.vue';

export default {
  name: 'Header',
  component: {
    Head,
  },
};
</script>

<style scoped>
.header {
  border-bottom: 1px solid #e8e8e8;
}
.head {
  padding-top: 3.2em;
  height: 6.187em;
  border-bottom: 1px solid #e8e8e8;
}

.user {
  width: 990px;
  position: absolute;
  justify-content: flex-end;
  display: flex;
  flex-direction: row;
  top: 20px;
  left: 50%;
  transform: translate(-50%, 0%);
}
.user-lang {
  width: 70px;
  font-size: 13px;
}
.user-lang::after {
    width: 8px;
    height: 5px;
    content: "";
    background-image: url("https://res.kurly.com/pc/ico/1908/ico_down_8x5.png");
    position: absolute;
    background-repeat: no-repeat;
    margin: 8px 0 0 12px;
}
.user-login {
  width: 50px;
  font-size: 13px;
}

.head-inner {
  width: 990px;
  margin: 0 auto;
  display: flex;
  flex-direction: row;
}
.logo {
  margin: 5px 35px 0 0;
}

.search {
  width: 478px;
  height: 46px;
  border: 1px solid black;
  display: flex;
  flex-direction: row;
}
.search-inner {
  width: 429px;
  height: 46px;
  padding: 0 0 0 10px;
  font-size: 16px;
  outline: none;
  border: none;
}
.search-btn {
  width: 30px;
  height: 30px;
  border: none;
  outline: none;
  padding: 0;
  background-color: rgba(0, 0, 0, 0);
  cursor: pointer;
  margin: 10px;
}
.search-btn-img {
  width: 24px;
  height: 24px;
}

.navi {
  width: 990px;
  margin: 0 auto;
}
.navi-inner {
  margin: 5px 0 5px 0;
}
.navi-list {
  margin: 0;
  padding: 5px 0 5px 0;
  list-style: none;
  display: flex;
  flex-direction: row;
}
.navi-list-txt {
  margin: 5px 0 5px 0;
}
.navi-list-arrow {
  font-size: 14px;
  margin: 0 6px 0 8px;
}
</style>
