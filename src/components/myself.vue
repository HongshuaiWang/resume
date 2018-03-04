<template>
  <el-container class="myself-container">
    <el-main class="myself-main">
      <div class="myself myself-name">
        <div class="avatar"><img src="@/assets/avatar.png" alt="照片头像" /></div>
        <h2>王洪帅</h2>
        <h3>Web前端开发工程师</h3>
      </div>
      <div class="myself myself-base-info">
        <el-row class="myself-info base-info">
          <el-col>
            <div>男 / 1991.02</div>
          </el-col>
        </el-row>
        <el-row class="myself-info base-info">
          <el-col>
            <div>吉林大学 · 信息管理与信息系统</div>
          </el-col>
        </el-row>
        <el-row class="myself-info base-info">
          <el-col>
            <div>本科 / 2014年毕业</div>
          </el-col>
        </el-row>
        <el-row class="myself-info base-info">
          <el-col>
            <div>期望工作地点：广东 · 深圳</div>
          </el-col>
        </el-row>
        <el-row class="myself-info base-info">
          <el-col>
            <div>当前居住地址：山东 · 青岛</div>
          </el-col>
        </el-row>
        <el-row class="myself-info base-info">
          <el-col>
            <a href="mailto:hongshuai_wang@qq.com" target="_blank"><i class="el-icon-message">&nbsp;&nbsp;hongshuai_wang@qq.com</i></a>
          </el-col>
        </el-row>
        <el-row class="myself-info base-info">
          <el-col>
            <a href="tel:18562532250"><i class="el-icon-phone">&nbsp;&nbsp;185-6253-2250</i></a>
          </el-col>
        </el-row>
      </div>
      <div class="myself myself-skills">
        <div class="myself-info">
          <div>HTML</div>
          <el-progress :show-text="false" :stroke-width="10" :percentage="80"></el-progress>
        </div>
        <div class="myself-info">
          <div>Javascript</div>
          <el-progress :show-text="false" :stroke-width="10" :percentage="80"></el-progress>
        </div>
        <div class="myself-info">
          <div>CSS</div>
          <el-progress :show-text="false" :stroke-width="10" :percentage="70"></el-progress>
        </div>
        <div class="myself-info">
          <div>Java</div>
          <el-progress :show-text="false" :stroke-width="10" :percentage="60"></el-progress>
        </div>
        <div class="myself-info">
          <div>C# / Silverlight</div>
          <el-progress :show-text="false" :stroke-width="10" :percentage="90"></el-progress>
        </div>
        <div class="myself-info">
          <div>Oracle / Mysql</div>
          <el-progress :show-text="false" :stroke-width="10" :percentage="70"></el-progress>
        </div>
      </div>
    </el-main>
  </el-container>
</template>

<style>
.myself-container {
  height:100%;
}

.avatar {
  width: 200px;
  margin: 0 auto;
}

.avatar img {
  width: 200px;
  border-radius: 50%;
}

.myself-name {
  text-align: center;
}

.myself-name h2 {
  font-size: 3rem;
  letter-spacing: 5px;
  font-family: sans-serif;
}

.myself-name h2, .myself-name h3 {
  color: #00b38a;
  font-weight: normal;
  font-family: 'Trebuchet MS', Helvetica, sans-serif;
}

.myself {
  margin-bottom: 50px;
}

.myself-info  {
  color: #999;
  margin-bottom: 10px;
}

.myself-info.base-info {
  color: #555;
}

.myself-info div:first-child {
  padding: 1px;
}

.myself-info .el-progress-bar__outer {
  background-color: #d7d7d7;
}

.myself-info .el-progress-bar__inner {
  background-color: #00b38a;
}

.myself-info a:link {
  display: block;
  margin-top: 10px;
  color: #333;
}

.myself-info a:hover {
  color: #999;
}

</style>