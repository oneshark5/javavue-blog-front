<!-- 首页 -->
<template>
    <div>
        <!-- 顶部导航栏 -->
        <navbar></navbar>
        <!-- 中间内容 -->
        <div class="container">
            <el-row  :gutter="30">
                <el-col :sm="24" :md="16" style="transition:all .5s ease-out;margin-bottom:30px;">
                    <!-- 左侧文章 -->
                    <articlelist></articlelist>
                </el-col>
                <el-col :sm="24"  :md="8" >
                    <!-- 右侧侧边栏 -->
                    <rightlist></rightlist>
                </el-col>
            </el-row>
        </div>
    </div>
</template>

<script>
import header from "../components/header.vue";
import articlelist from "../components/articlelist.vue";
import rightlist from "../components/rightlist.vue";
export default {
  name: "Home",
  data() {
    //选项 / 数据
    return {};
  },
  methods: {
    //事件处理器
  },
  components: {
    //定义组件
    navbar: header,
    articlelist: articlelist,
    rightlist: rightlist
  },
  created() {
    //生命周期函数
  }
};
</script>

<style>
</style>
