
<template>
  <div id="app">
    <div class="vue_radio">
      <div class="tabs">

        <input type="radio" id="tab1" value="1" v-model="isActive">
        <label for="tab1">タブメニュー1</label>

        <input type="radio" id="tab2" value="2" v-model="isActive">
        <label for="tab2">タブメニュー2</label>

        <input type="radio" id="tab3" value="3" v-model="isActive">
        <label for="tab3">タブメニュー3</label>

      </div>
      <ul class="contents">
        <li v-if="isActive === '1'">コンテンツ１コンテンツ１コンテンツ１コンテンツ１コンテンツ１コンテンツ１</li>

        <li v-if="isActive === '2'">コンテンツ２コンテンツ２コンテンツ２コンテンツ２コンテンツ２コンテンツ２</li>

        <li v-if="isActive === '3'">コンテンツ３コンテンツ３コンテンツ３コンテンツ３コンテンツ３コンテンツ３</li>
      </ul>
    </div>
  </div>    
  </template>