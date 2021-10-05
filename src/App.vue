<template>
  <div id="app">
    <student v-for="student in studentList" :key="student.id"
    :photoStudent="student.photoStudent"
    :nameStudent="student.nameStudent"
    :studentAddress="student.studentAddress"
    />
  </div>
</template>

<script>
import Student from './components/Student'

export default {
  name: 'App',
  components: {
    Student
  },

  data() {
    return {
      studentList: [
        {
          photoStudent: "",
          nameStudent: "Ігор",
          studentAddress: "Ужгород"
        },
        {
          photoStudent: "",
          nameStudent: "Євген",
          studentAddress: "Чоп"
        }
      ]
    }
  }
}
</script>

<style>

</style>
