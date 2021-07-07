<template>
    <div class="header">
      <div class="head">
        <UserMenu/>
        <div class="head-inner">
          <a href="https://cs.kakao.com/" class="logo">
            <img src="https://cs.kakao.com/img/cskakaocom/pc/tit_cs2.gif">
          </a>
          <Search/>
        </div>
      </div>
      <Navi/>
    </div>
</template>

<script>
import UserMenu from './UserMenu.vue';
import Search from './Search.vue';
import Navi from './Navi.vue';

export default {
  name: 'Header',
  components: {
    UserMenu,
    Search,
    Navi,
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
.head-inner {
  width: 990px;
  margin: 0 auto;
  display: flex;
  flex-direction: row;
}
.logo {
  margin: 5px 35px 0 0;
}
</style>
