<template>
    <div class="search">
        <input class="search-inner" type="search" placeholder="궁금한 점이 있다면 도움말을 검색해 보세요.">
        <button class="search-btn">
            <img width="24" height="24" src="https://www.seekpng.com/png/full/871-8719667_download-png-transparent-background-search-icon.png">
        </button>
    </div>
</template>

<script>
export default {
  name: 'Search',
  components: {
  },
};
</script>

<style scoped>
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
</style>
