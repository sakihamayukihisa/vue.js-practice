<template>
  <div id="app">
    <div class="vue_radio">
      <div class="tabs">
        <input type="radio" id="tab1" value="1" v-model="isActive" />
        <label for="tab1">タブメニュー1</label>
        <input type="radio" id="tab2" value="2" v-model="isActive" />
        <label for="tab2">タブメニュー2</label>
        <input type="radio" id="tab3" value="3" v-model="isActive" />
        <label for="tab3">タブメニュー3</label>
      </div>
      <ul class="contents">
        <li v-if="isActive === '1'">コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1</li>
        <li v-else-if="isActive === '2'">コンテンツ2コンテンツ2コンテンツ2コンテンツ2コンテンツ2コンテンツ2コンテンツ2コンテンツ2</li>
        <li v-else-if="isActive === '3'">コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: "1"
    };
  }
};
</script>

<style>
.tabs label {
  padding: 5px 20px;
  cursor: pointer;
}
.tabs :checked + label {
  background-color: #000;
  color: #fff;
}
input {
  display: none;
}
ul {
  margin: 0;
  padding: 0;
}
li {
  list-style: none;
  width: 500px;
  padding: 20px;
  border: 1px solid #ccc;
}
</style>