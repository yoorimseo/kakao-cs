<template>
  <div class="snb">
    <h2 class="snb-title">카카오톡 지갑</h2>
    <ul class="snb-list">
      <li class="snb-list-txt"
        v-for="categoryName in categoryNameList" :key="categoryName"
        @click="changeCategory(categoryName)"
        :class="{'snb-list-selected-txt': selectedCategory}"
      >{{categoryName}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'SNB',
  props: ['categoryNameList', 'changeCategory'],
  data() {
    return {
      selectedCategory: false,
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
.snb-list-selected-txt {
  color: black;
}
</style>
