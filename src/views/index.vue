<template>
  <div id="index">
    <el-row class="tac">
      <el-col :span="4">
        <v-nav></v-nav>
      </el-col>
      <el-col :span="18">
        <v-table></v-table>
      </el-col>
    </el-row>
  </div>
</template>

<script>
  import Nav from '../components/nav.vue'
  import Table from '../components/table.vue'
    export default {
      name: "Index",
      components:{
        'v-nav':Nav,
        'v-table':Table
      },
      data(){
        return{}
      },
      mounted: function() {
        this.$nextTick(function () {    //vue初始化加载方法
        })
      },
      methods: {
        tableRowClassName({row, rowIndex}) {
          if (rowIndex === 1) {
            return 'warning-row';
          } else if (rowIndex === 3) {
            return 'success-row';
          }
          return '';
        }
      }
    }
</script>

<style scoped>

</style>
