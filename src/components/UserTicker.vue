<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 135****9901 完成了职场 3 年产品经理成长履历与能力复盘"
  },
  {
    "text": "用户 189****3312 生成了大学四年学业、社团与实习里程碑总结"
  },
  {
    "text": "用户 131****7780 完成了创业 2 年项目成败复盘与认知升级"
  },
  {
    "text": "用户 158****2219 生成了 30 岁人生立点与下半场规划指导"
  },
  {
    "text": "用户 173****8890 取得了年度个人读写、健康与财富全方位总结"
  }
]);
</script>
