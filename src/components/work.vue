<template>
  <el-container>
    <card :cardType="cardType" :title="title" :items="items"/>
  </el-container>
</template>

<script>
import card from '@/components/widgets/card'
export default {
  name: 'work',
  components: {
    'card': card
  },
  data() {
    return {
      cardType: 'title-list',
      title: '工作经历',
      items: [{
        daterange: '2014.08 ~ 至今',
        title: '青岛海信智能商用系统股份有限公司',
        content: [{
          key: '',
          value: '主要负责快速开发平台FDP3.0的开发与维护、FDP4.0报表系统的设计开发与维护、海信银联卡受理终端管理系统的设计开发与维护，参与通用通讯平台CTP3.0的开发与维护、 HIAIP应用集成平台的开发与维护，对快速开发平台FDP4.0进行mysql支持改造等'
        }]
      }]
    }
  }
}
</script>