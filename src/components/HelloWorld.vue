<template>
  <el-button @click="testMsg">Click</el-button>
</template>

<script lang="ts">
import {defineComponent} from "vue";
import 'element-plus/theme-chalk/el-message.css';
import { ElMessage } from 'element-plus';

export default defineComponent({
  name: "HelloWorld",
  methods: {
    testMsg() {
      ElMessage({
        showClose: true,
        message: 'test',
        center: true,
        type: 'success',
      });
    }
  }
});
</script>
