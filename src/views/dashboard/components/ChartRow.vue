<!--
 * @Author: your name
 * @Date: 2021-01-04 09:52:23
 * @LastEditTime: 2021-01-04 17:39:45
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: \vue-elment-admin\src\views\dashboard\components\ChartRow.vue
-->
<template>
  <el-row :gutter="32">
    <el-col
      :xs="24"
      :sm="24"
      :lg="8"
    >
      <div class="chart-wrapper">
        <RaddarChart />
      </div>
    </el-col>
    <el-col
      :xs="24"
      :sm="24"
      :lg="8"
    >
      <div class="chart-wrapper">
        <PieChart />
      </div>
    </el-col>
    <el-col
      :xs="24"
      :sm="24"
      :lg="8"
    >
      <div class="chart-wrapper">
        <BarChart />
      </div>
    </el-col>
  </el-row>
</template>

<script>
import RaddarChart from '@/components/Chart/RaddarChart'
import PieChart from '@/components/Chart/PieChart1'

// import PieChart from '@/components/Chart/PieChart'
import BarChart from '@/components/Chart/BarChart'

export default {
  name: 'ChartRow',
  components: {
    RaddarChart,
    PieChart,
    BarChart
  },
  data() {
    return {}
  },
  mounted() {},
  methods: {}
}
</script>

<style scoped>
  .chart-wrapper {
    background: #fff;
    padding: 16px 16px 0;
    margin-bottom: 32px;
  }

  @media (max-width: 1024px) {
    .chart-wrapper {
      padding: 8px;
    }
  }
</style>
