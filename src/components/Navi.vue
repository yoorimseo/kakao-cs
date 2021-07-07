<template>
    <div class="navi">
        <div class="navi-inner">
            <ul class="navi-list">
                <li class="navi-list-txt" v-for="(link, idx) in naviLink" v-bind:key="idx">
                    <a href="#">{{link}}</a>
                    <span class="navi-list-arrow" v-if="idx < naviLink.length-1">></span>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Navi',
  data() {
    return {
      naviLink: ['홈', '카카오톡 지갑', '일반'],
    };
  },
};
</script>

<style scoped>
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
.navi-list li a:hover {
    text-decoration: 1px black underline;
}
.navi-list-txt {
  margin: 5px 0 5px 0;
}
.navi-list-arrow {
  font-size: 14px;
  margin: 0 6px 0 8px;
  color: #777;
}
</style>
