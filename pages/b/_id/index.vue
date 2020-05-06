<template>
  <div class="container">
    <!-- <h1 class="board__title title has-text-centered">안녕하세요</h1>
    <span class="date">2020-05-05 16:13:11</span>
    <div class="columns">
      <div class="column is-two-thirds">
        <div class="level is-small">
          <div class="level-item has-text-centered">
            <div>
              <p class="heading">조회수</p>
              <p class="title">12</p>
            </div>
          </div>
          <div class="level-item has-text-centered">
            <div>
              <p class="heading">추천수</p>
              <p class="title">3</p>
            </div>
          </div>
        </div>
      </div>
    </div> -->
    
    <article class="message is-dark">
      <div class="message-header">
        <h1 class="board__title title has-text-centered">안녕하세요</h1>
        <!-- <i class="fas fa-thumbs-up"></i> -->
      </div>
      <div class="message-body is-clearfix">
        <div>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. <strong>Pellentesque risus mi</strong>, tempus quis placerat ut, porta nec nulla. Vestibulum rhoncus ac ex sit amet fringilla. Nullam gravida purus diam, et dictum <a>felis venenatis</a> efficitur. Aenean ac <em>eleifend lacus</em>, in mollis lectus. Donec sodales, arcu et sollicitudin porttitor, tortor urna tempor ligula, id porttitor mi magna a neque. Donec dui urna, vehicula et sem eget, facilisis sodales sem.
        </div>
        <span class="date is-pulled-right">world<br>2020-05-05 16:13:11</span>
      </div>
    </article>

    <div class="level is-small">
      <div class="level-item has-text-centered">
        <div>
          <p class="heading">조회수</p>
          <p class="title">12</p>
        </div>
      </div>
      <div class="level-item has-text-centered">
        <div>
          <p class="heading">추천수</p>
          <p class="title"><a href="#" ><i class="far fa-thumbs-up"></i></a> 3</p>
        </div>
      </div>
    </div>

    <Reply />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Reply from '~/components/Reply.vue';
export default Vue.extend({
  components: {
    Reply
  }
})
</script>

<style lang='scss'>
  .board__title{
    color: #fff;
  }
  .board__contents{
    padding: 2.5rem 1.25rem;
  }
  .level{
    border-bottom: 1px solid #dbdbdb;
    padding-bottom: 2rem;
  }
  .date{
    padding-top: 2rem;
  }
</style>
