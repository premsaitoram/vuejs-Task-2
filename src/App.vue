

<template>
  <div>
    <Header theTitle="Vue Data"/>
   <TaskList theTitle = "My Tasks" v-bind:taskList="tasks"/>
  </div>
  
</template>
<script>
import Header from './components/Header.vue'
import TaskList from './components/TaskList.vue'
export default {
  name:'App' ,
  components: {
    Header,
    TaskList
  },
  data(){
    return{
      tasks:[
        {id:1, title:"Learn HTML&CSS", completed:false,},
        {id:2, title:"Learn JavaScript", completed:true,},
        {id:3, title:"Learn Vue JS", completed:false,}
      ]
    }
  }
}
</script>


<style>
*{
  margin:0;
  padding: 0;
}
</style>
