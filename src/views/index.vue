<template>
  <div id="index">
    <el-row class="tac">
      <el-col :span="4">
        <v-nav v-on:nav_index="navNum"></v-nav>
      </el-col>
      <el-col :span="18">
        <v-table_main v-if="main_show.table_show"></v-table_main>
      </el-col>
    </el-row>
  </div>
</template>

<script>
  import Nav from '../components/nav.vue'
  import Table_box from '../components/table_main.vue'
    export default {
      name: "Index",
      components:{
        'v-nav':Nav,
        'v-table_main':Table_box
      },
      data(){
        return{
          main_show:{
            table_show:true,
            student_data_show:false
          }
        }
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
        },
        navNum:function(itme){
          if(itme == 1){

          }
        }
      }
    }
</script>

<style scoped>

</style>
