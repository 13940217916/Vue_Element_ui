<template>
  <div class="nav">
    <h5>Element ui</h5>
    <el-menu
      default-active="1"
      class="el-menu-vertical-demo"
      text-color="#545c64"
      active-text-color="#ffd04b">
      <el-menu-item v-bind:index=x.order v-for="(x,index) in nav_data" v-on:click="tab_nav(x)">
        <span slot="title">{{x.name}}</span>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
    export default {
      name: "nav_bar",
      data(){
        return{
          nav_data:[
            {
              order:'1',
              name:'学生信息'
            },
            {
              order:'2',
              name:'新生信息录入'
            },
            {
              order:'3',
              name:'课程表信息'
            }
          ]
        }
      },
      methods:{
        tab_nav:function(item){
          var nav_index = item.order
          this.$emit("nav_index",nav_index)
        }
      }
    }
</script>

<style scoped>

</style>
