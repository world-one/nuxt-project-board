<template>
  <div class="container container__height">
    <table class="main__table table is-fullwidth is-hoverable has-text-centered">
      <thead>
        <tr>
          <th>번호</th>
          <th>제목</th>
          <th>날짜</th>
          <th>조회수</th>
          <th>추천수</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, index) in list" :key="index">
          <td>{{item.id}}</td>
          <td><nuxt-link :to="{name:'b-id',params:{ id : item.id }}">{{item.title}}</nuxt-link></td>
          <td>{{item.date}}</td>
          <td>{{item.views}}</td>
          <td>{{item.recomm}}</td>
        </tr>
      </tbody>
    </table>
    
    <nav class="pagination is-centered" role="navigation" aria-label="pagination">
      <a class="pagination-previous">Previous</a>
      <a class="pagination-next">Next page</a>
      <ul class="pagination-list">
        <li><a class="pagination-link" aria-label="Goto page 1">1</a></li>
        <li><span class="pagination-ellipsis">&hellip;</span></li>
        <li><a class="pagination-link" aria-label="Goto page 45">45</a></li>
        <li><a class="pagination-link is-current" aria-label="Page 46" aria-current="page">46</a></li>
        <li><a class="pagination-link" aria-label="Goto page 47">47</a></li>
        <li><span class="pagination-ellipsis">&hellip;</span></li>
        <li><a class="pagination-link" aria-label="Goto page 86">86</a></li>
      </ul>
    </nav>
    <div class="field has-addons has-addons-centered">
      <div class="control">
        <input class="input" type="text" placeholder="Find a repository">
      </div>
      <div class="control">
        <a class="button is-info">
          Search
        </a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'


export default Vue.extend({
  data() {
    return {
      list: [
        {
          id : 1,
          title : '안녕하세요',
          date : '2020-05-06',
          views : 3,
          recomm: 2
        },
        {
          id : 2,
          title : '안녕하세요22',
          date : '2020-05-06',
          views : 3,
          recomm: 2
        }
      ]
    }
  },
  components: {
    
  }
})
</script>

<style lang="scss">
@import '~/assets/scss/page/main.scss';
</style>
