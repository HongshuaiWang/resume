<template>
  <div>
    <el-row class="item-title">
      <el-col :xs="10" :sm="10" :md="9" :lg="9" :xl="9">
        <div>{{ daterange }}</div>
      </el-col>
      <el-col :xs="14" :sm="14" :md="15" :lg="15" :xl="15">
        <div>{{ itemTitle }}</div>
      </el-col>
    </el-row>
    <el-row class="item-content" v-for="content in itemContent" :key="content">
      <div v-if="content.key" class="item-content-list">
        <el-col :xs="7" :sm="6" :md="5" :lg="4" :xl="2">
          <div>{{ content.key }}</div>
        </el-col>
        <el-col :xs="17" :sm="18" :md="19" :lg="20" :xl="22">
          <div>{{ content.value }}</div>
        </el-col>
      </div>
      <div v-else class="item-content-list item-content-no-key">
        <el-col>
          <div>{{ content.value }}</div>
        </el-col>
      </div>
    </el-row>
  </div>
</template>

<script>
export default {
  props: {
    daterange: {
      type: String,
      required: true
    },
    itemTitle: {
      type: String,
      required: true
    },
    itemContent: {
      type: Array,
      required: true
    }
  }
}
</script>