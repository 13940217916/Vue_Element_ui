<template>
  <div id="table_box">
    <el-table :data="tableData2" stripe border style="margin: 60px 0 0 20px;">
      <el-table-column label="学号" prop="code" width="180" align="center"></el-table-column>
      <el-table-column label="日期" prop="date" width="180" align="center"></el-table-column>
      <el-table-column label="姓名" prop="name" width="180" align="center"></el-table-column>
      <el-table-column label="地址" prop="address" width="300" align="center"></el-table-column>
      <el-table-column fixed="right" label="操作" align="center">
        <template slot-scope="scope">
          <el-button type="text" size="small">查看</el-button>
          <el-button type="text" size="small">编辑</el-button>
        </template>
      </el-table-column>
    </el-table>
    <el-pagination
      style="float: left;margin:20px 0 0 10px"
      background
      layout="prev, pager, next"
      :total="100">
    </el-pagination>
  </div>

</template>

<script>
    export default {
      name: "table_main",
      data(){
          return{
            tableData2: [{
              date: '2016-05-02',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄',
            }, {
              date: '2016-05-04',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄'
            }, {
              date: '2016-05-01',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄',
            }, {
              date: '2016-05-03',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄'
            }, {
              date: '2016-05-01',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄',
            }, {
              date: '2016-05-01',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄',
            }, {
              date: '2016-05-01',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄',
            }, {
              date: '2016-05-01',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄',
            }, {
              date: '2016-05-01',
              name: '王小虎',
              code:18021,
              address: '上海市普陀区金沙江路 1518 弄',
            },
            ]
          }
      }
    }
</script>

<style scoped>

</style>
