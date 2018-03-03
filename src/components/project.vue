<template>
  <el-container>
    <card :cardType="cardType" :title="title" :items="items"/>
  </el-container>
</template>

<script>
import card from '@/components/widgets/card'
export default {
  name: 'project',
  components: {
    'card': card
  },
  data() {
    return {
      cardType: 'title-list',
      title: '项目经历',
      items: [{
	      daterange: '2017.03 ~ 2017.07',
	      title: '海信银联卡受理终端管理系统',
	      content: [{
          key: '项目描述：',
          value: '主要包含终端联机激活，终端序列号密钥生成、灌装与导出，应用网签系统三大部分。涉及与加密机通过socket交互、提供服务接口供客户端调用、以及后台管理系统等开发'
        }, {
          key: '责任描述：',
          value: '主导项目设计开发工作。具体负责项目整体的需求分析与评估，负责mysql数据库设计、开发与备份工作，服务端接口设计与开发，后台管理系统设计与开发，以及后续的维护与新需求扩展'
        }, {
          key: '主要技术：',
          value: 'js+html+css、java（springmvc）、mysql，通过tomcat部署'
        }]
      }, {
        daterange: '2017.05 ~ 2017.11',
        title: '通用通讯平台CTP3.0 / HIAIP应用集成平台',
        content: [{
          key: '项目描述：',
          value: 'CTP项目主要采用增量的方式自动化对数据进行上传下载工作；HIAIP项目主要是集成线上业务，如扫码支付、线上订单等'
        }, {
          key: '责任描述：',
          value: 'CTP项目主要负责服务端的开发与维护，对重构的功能代码进行检查；HIAIP项目主要参与支付部分对接与测试，例如微信支付、支付宝支付等。同时对两个项目web端进行部分设计与开发，协助组内员工完成部分分析工作'
        }, {
          key: '主要技术：',
          value: 'js+html+css、java（springmvc）、oracle'
        }]
      }, {
        daterange: '2016.08 ~ 2017.02',
        title: 'FDP4.0报表系统',
        content: [{
          key: '项目描述：',
          value: '基于FDP4.0快速开发平台开发的报表系统，基于存储过程作为数据源，存储过程参数、结果集分别对应报表查询条件和数据展示，可对接其他任意业务系统，提供报表设计、报表展示（查询方案+图形+表格）的功能'
        }, {
          key: '责任描述：',
          value: '作为项目负责人，主要对报表设计的步骤流程、数据库、缓存数据库（mongodb）、服务端逻辑及接口进行设计与开发，同时开发web端报表设计界面和部分报表展界面开发与优化；带徒弟参与项目并进行子方案设计、方案评审和代码review等'
        }, {
          key: '主要技术：',
          value: 'js+html+css、java（springmvc）、MongoDB、oracle/mysql'
        }]
      }, {
        daterange: '2014.08 ~ 至今',
        title: '快速开发平台FDP3.0',
        content: [{
          key: '项目描述：',
          value: '采用微软silverlight+C#+WCF+IIS开发的平台，提供底层控件组件、模板页（单表、一主一从、一主多从等）、业务基类，同时提供用户权限管理模型，完备的增删改查、列校验行校验、参照等等底层逻辑，业务开发人员仅需简单配置即可实现简单的业务界面和逻辑控制，同时有很好的扩展性'
        }, {
          key: '责任描述：',
          value: '作为项目负责人，主要对该项目进行新需求开发以及缺陷跟踪修复、数据库等性能调优，同时对业务开发人员、客户等提供相应的解决方案与技术支持工作；带徒弟参与项目并进行方案设计、方案评审和代码review等'
        }, {
          key: '主要技术：',
          value: 'silverlight、C#、WCF、oracle'
        }]
      }]
    }
  }
}
</script>