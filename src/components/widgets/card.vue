<template>
  <el-card class="box-card">
    <div slot="header" class="section-header">
      <h2 class="section-title">{{ title }}</h2>
    </div>
    <div class="section-contont">
      <div v-if="cardType==='title-list'" v-for="item in items" :key="item.title">
        <title-list :daterange="item.daterange" :itemTitle="item.title" :itemContent="item.  content" class="items" :class="{ 'multi-title-items': items.indexOf(item) !== items.length - 1 }"/>
      </div>
      <ul v-if="cardType==='unordered-list'" >
        <li v-for="item in items" :key="item" class="items item-content" v-html="item"></li>
      </ul>
    </div>
  </el-card>
</template>

<script>
import titleList from '@/components/widgets/title-list'

export default {
  components: {
    'title-list': titleList
  },
  props: {
    cardType: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    items: {
      type: Array,
      required: true
    }
  }
}
</script>

<style>
.box-card {
  width: 100%;
}

.section-title {
  width: 30%;
  min-width: 150px;
  margin: 0 auto;
  text-align: center;
  background-color: #eee;
  border-radius: 32px;
  padding: 4px 10px;
  font-size: 1rem;
  font-weight: normal;
}

.items {
  margin: 10px 20px;
}

li.items {
  list-style-position: inside;
  margin: 5px 20px;
}

.item-title, .item-content {
  word-wrap: break-word;
  font-size: 0.9rem;
}

.item-content-list {
  margin-top: 5px;
}

.item-content-no-key div:first-letter {
  padding: 0 0 0 1.8rem;
}

.multi-title-items:after {
  content: ' ';
  margin-top: 10px;
  display: block;
  width: 100%;
  height: 1px;
  background: #999;
}

</style>