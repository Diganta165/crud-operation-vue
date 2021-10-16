<template>
  <div>
    <h1>Add Employee</h1>
    <form @submit.prevent="handleEmployee">
      <input type="text" v-model="employee.employeeName" placeholder="Name" />
      <input type="text" v-model="employee.employeeEmail" placeholder="Email" />
      <input type="submit" value="submit" />
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      employee: {
        employeeName: "",
        employeeEmail: ""
      },
    };
  },
  methods:{
    handleEmployee(){
      // console.log(this.employee.employeeName, this.employee.employeeEmail)
      this.$emit('add:employeeInfo',this.employee)
    }
  }
};
</script>

<style>
</style>