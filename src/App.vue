<template>
  <HeaderTitle title="Task Tracker" />
  <TasksList :tasks="tasks" />

</template>

<script>

  import HeaderTitle from './components/Header'
  import TasksList from './components/Tasks'


export default {
  name: 'App',
  components: {
    HeaderTitle,
    TasksList,
  },

  data(){
    return{
      tasks: [],
    }
  },

  created(){
    this.tasks = [
      {
        id: 1,
        title: 'Learn Vue',
        day: 'Monday',
        completed: false,
      },
      {
        id: 2,
        title: 'Take the trash out',
        day: 'Sunday',
        completed: true,
      },
      {
        id: 3,
        title: 'Gym',
        day: 'Friday',
        completed: false,
      },
    ]
  },
  }

</script>
<style>
#app {
  font-family: 'Helvetica';
  font-size: 10px;
  color: #333;
  background-color: #eee;
  padding: 1rem;

}
</style>
