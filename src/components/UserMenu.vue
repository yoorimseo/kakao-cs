<template>
    <div class="user-menu">
        <div class="user-lang">
            <span>한국어</span>
        </div>
        <div class="user-login">
            <span>로그인</span>
        </div>
    </div>
</template>

<script>
export default {
  name: 'UserMenu',
  components: {
  },
};
</script>

<style scoped>
.user-menu {
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
  cursor: pointer;
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
  cursor: pointer;
}
</style>
