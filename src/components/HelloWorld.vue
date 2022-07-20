<template>
  <el-tabs v-model="activeName" class="demo-tabs" @tab-click="handleClick">
    <el-tab-pane label="User" name="first">
      first
      <el-tooltip placement="top">
        <div style="width: 100px; height: 1000px">1234567890</div>
        <template #content>
          <div style="font-size: 16px">啦啦啦啦啦啦</div>
        </template>
      </el-tooltip>
    </el-tab-pane>
    <el-tab-pane label="Config" name="second">
      second
      <el-tooltip placement="top">
        <div style="width: 100px; height: 1000px">1234567890</div>
        <template #content>
          <div style="font-size: 16px">啦啦啦啦啦</div>
        </template>
      </el-tooltip>
    </el-tab-pane>
    <el-tab-pane label="Role" name="third">Role</el-tab-pane>
    <el-tab-pane label="Task" name="fourth">Task</el-tab-pane>
  </el-tabs>
</template>

<script setup>
import { ref } from 'vue';

const activeName = ref('first');
console.error(activeName);
const handleClick = (tab, event) => {
  console.log(tab, event);
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
