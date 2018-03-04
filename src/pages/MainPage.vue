<template>
  <el-container class="resume-container">
    <el-main class="resume-main">
      <work class="resume-section"/>
      <project class="resume-section"/>
      <skill class="resume-section"/>
      <commit class="resume-section"/>
    </el-main>
    <el-aside class="resume-aside" width="">
      <myself/>
    </el-aside>
    <a class="pdf-resume-download" href="/static/简历_王洪帅.pdf"><el-button type="primary" icon="el-icon-download">PDF简历</el-button></a>
  </el-container>
</template>

<script>
import myself from '@/components/myself'
import work from '@/components/work'
import project from '@/components/project'
import skill from '@/components/skill'
import commit from '@/components/commit'

export default {
  name: 'MainPage',
  components: {
    'work': work,
    'project': project,
    'skill': skill,
    'commit': commit,
    'myself': myself
  },
  data() {
    return {
          
    }
  }
}
</script>

<style>
html {
  font-size: 16px;
}

body {
	background-color: #eee;
}

.resume-container {
	width:70%;
	margin: 10px auto;
  -webkit-box-shadow: #888888 0 0 10px;
  -moz-box-shadow: #888888 0 0 10px;
	box-shadow: #888888 0 0 10px;
  -webkit-border-radius: 4px;
  -moz-border-radius: 4px;
  border-radius: 4px;
}

.resume-section {
	margin-bottom: 10px;
}

.resume-main {
	background-color: white;
  width: 70%;
}

.pdf-resume-download {
  position: fixed;
  bottom: 5px;
  right: 5px;
}

@media screen and (max-width: 1200px) {
  .resume-container {
    width:80%;
  }
}

@media screen and (max-width: 992px) {
  html {
    font-size: 14px;
  }
  .resume-container {
    width:100%;
  }

  .resume-aside {
    position: absolute;
    top: 0;
    background-color: #eee;
    width: 100%;
    margin: 0 auto;
    text-align: center;
  }

  .resume-aside .myself-skills {
    display: none;
  }

  .resume-main {
    background-color: white;
    position: absolute;
    top: 762px;
    width: 100%;
    padding: 0;
  }
}

@media screen and (max-width: 768px) {
  html {
    font-size: 12px;
  }
}

@media print {
  @page {
    size: A4;
    margin: 1.6cm 1cm;
  }

  html {
    font-size: 10px;
  }

  .resume-container {
    width:210mm;
  }

  .el-card__header {
    padding: 10px 20px;
  }

  .avatar img {
    padding: 15px;
  }

  .item-title .el-col:first-child {
    width: 40%;
  }

  .item-title .el-col:last-child {
    width: 60%;
  }

  .item-content .el-col:first-child {
    width: 15%;
  }

  .item-content .el-col:last-child {
    width: 85%;
  }

}
</style>