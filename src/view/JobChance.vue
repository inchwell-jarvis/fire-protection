<template>
  <div id="JobChance">
    <div class="banner container-fuild text-center">工作机会</div>
    <div class="container">
      <div class="JobChance-container wow pulse">
        <h2>消防安全检测员</h2>
        <p>岗位职责</p>
        <ol>
          <li>负责进行建筑、设施等场所的消防安全检测工作，确保符合相关法规和标准；</li>
          <li>执行消防安全检测计划，评估火灾风险，提供相应的改善建议；</li>
          <li>协助相关团队进行任务分配与监督，及时解决检测过程中的技术问题；</li>
          <li>参与建筑消防系统的需求分析与设计，负责完成检测相关的工作，制定检测标准和流程。</li>
        </ol>
        <p>任职要求</p>
        <ol>
          <li>具备扎实的消防安全理论知识，熟悉建筑消防安全检测流程和方法；</li>
          <li>有3年以上建筑消防安全检测经验，有大型建筑或公共场所检测经验者优先；</li>
          <li>熟悉使用各种消防安全检测工具，具备良好的问题分析和解决能力；</li>
          <li>了解建筑消防系统的原理和技术，有相关证书者优先；</li>
          <li>熟悉各种检测报告和文档的编写，能够清晰、准确地记录检测过程和结果；</li>
          <li>对建筑消防系统的检测、排错等方面有经验，能够应对各种火灾风险。</li>
        </ol>

        <button class="center-block btn btn-warning btn-lg">投递简历</button>
      </div>
    </div>
  </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
  name: "JobChance",
  data() {
    return {};
  },
  mounted(){
    var wow = new WOW();
    wow.init();
  }
};
</script>
<style scoped>
.banner {
  color: #fff;
  font-size: 30px;
  height: 150px;
  line-height: 150px;
  background-image: url("../assets/img/banner_2.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: scroll;
  background-position: center center;
}
.JobChance-container {
  margin: 100px;
  padding: 30px;
  transition: all ease 0.5s;
  border: 1px dashed salmon;
}
.JobChance-container h2{
  color: rgb(255, 102, 19);
  font-weight: bolder;
  text-align: center;
}
.JobChance-container p{
font-size: 20px;
  color: rgb(255, 102, 19);
  font-weight: 700;
}
.JobChance-container ol{
    list-style-type: decimal;
    padding-left: 30px;
}
.JobChance-container ol>li{
    font-size: 14px;
    line-height: 2.7rem;
}
@media screen and (max-width: 997px) {
  .JobChance-container {
    margin: 20px 0;
    padding: 20px;
    border: 1px dashed salmon;
  }
}
</style>

