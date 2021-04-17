<template>
  <div class="container">
    <Header title="Task Tracker" />
    <Tasks :tasks="tasks" />
  </div>
</template>

<script>
import Header from "./components/Header";
import Tasks from "./components/Tasks";

export default {
  name: "App",
  components: {
    Header,
    Tasks
  },
  data() {
    return {
      tasks: []
    }
  },
  created() {
    this.tasks =[
      {
        id:1,
        text: 'Doctors Appointment',
        day: "March 1st at 2:30pm",
        reminder: true,
      },
      {
        id:2,
        text: 'Meeting',
        day: "March 2nd at 10:30am",
        reminder: true,
      },
    ]
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
button {
    width: 35%;
    height: 40%;
}
</style>
