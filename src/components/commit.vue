<template>
  <el-container>
    <card :cardType="cardType" :title="title" :items="items"/>
  </el-container>
</template>

<script>
import card from '@/components/widgets/card'
export default {
  name: 'commit',
  components: {
    'card': card
  },
  data() {
    return {
      cardType: 'unordered-list',
      title: '工作展望/自我评价',
      items: [
        '我对工作的展望：&nbsp;&nbsp;主攻前端，同时对后端等其他模块保持一定的接触。一方面不过度依赖于他人，另一方面可以更好的和其他模块的开发人员沟通交流，可高效解决问题',
        '我对工作的态度：&nbsp;&nbsp;高效完成本职工作，保持学习的热情与积极性，与其他同事交流协作、共同提升',
        '克服困难的途径：&nbsp;&nbsp;在遇到不熟悉或记忆不准确的知识点时，往往会去上网查找API以及一些技术博客，或翻阅书籍，常用技术定期复习巩固；在遇到技术难题时，往往会去csdn、stack overflow等查找相关的问题以及解决思路，然后结合实际问题情况触类旁通，对问题进行修改、测试、调优以解决实际问题',
        '开阔自己的视野：&nbsp;&nbsp;除了学习项目所需的新技术以外，关注知乎上关于前端等技术的专栏、话题，阿里技术、CSDN技术头条等微信公众号，喜欢在娱乐中学习等',
        '自己的优势：喜欢做技术、自学能力强，同时有较强的分析解决实际问题的能力，并逐步培养了自己在项目中的沟通协调能力',
        '自己的劣势：涉猎的技术虽然广泛但是深入度不够，从开始接触前端工作就深深喜欢上了，但是由于工作上的安排导致工作比较繁杂，还要对平台使用者提供各种解决方案/技术支持，一个人的精力始终是有限的，不能做到对某一个领域持久的学习、研究、运用，导致许多自学的新技术用的较少导致记忆不牢'
      ]
    }
  }
}
</script>