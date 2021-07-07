<template>
    <div class="footer">
        <div class="fnb">
            <div class="fnb-menu">
                <ul class="fnb-list">
                <li>회사소개</li>
                <li>이용약관</li>
                <li class="fnb-list-txt">개인정보처리방침</li>
                <li>운영정책</li>
                <li>청소년보호정책</li>
                <li>권리침해신고안내</li>
                <li>공지사항</li>
                </ul>
            </div>
            <div class="fnb-copy">
                <span>Copyright © Kakao Corp. All rights reserved.</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style scoped>
.footer {
  border-top: 1px solid #e8e8e8;
}

.fnb {
  width: 990px;
  height: 149px;
  margin: 0 auto;
  padding-top: 29px;
}
.fnb-menu {
  font-size: 13px;
  color: #787878;
}
.fnb-list {
  list-style: none;
  display: flex;
  flex-direction: row;
  padding: 0;
  margin: 0;
}
.fnb-list li {
  margin-right: 10px;
}
.fnb-list-txt {
  font-weight: 600;
}
.fnb-copy {
  margin-top: 28px;
  font-size: 13px;
  color: #787878;
}
</style>
