<template>
  <el-container>
    <card :cardType="cardType" :title="title" :items="items"/>
  </el-container>
</template>

<script>
import card from '@/components/widgets/card'
export default {
  name: 'skill',
  components: {
    'card': card
  },
  data() {
    return {
      cardType: 'unordered-list',
      title: '专业技能',
      items: [
        '前端技术：javascript、HTML、css',
        '前端框架及工具：了解并简单使用 MVVM框架 Vue、熟悉使用JQuery、requireJS等',
        '后端技术：java、springmvc',
        '数据库：较为熟练使用Oracle数据库、Mysql数据库，简单使用mongodb',
        '.net：熟练使用C#语言、silverlight等',
        '软实力：参与并带过几个项目，有较强的分析解决问题的能力以及学习能力，能有效的通过网上查找资料结合自身思考、通过测试验证等得出较优的解决方案'
      ]
    }
  }
}
</script>