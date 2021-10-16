<template>
  <div>
    <h1>This is Employees Component</h1>
    <employee-form-component @add:employeeInfo="updateEmployees"></employee-form-component>
    <!-- <employee-form-component v-on:employeeInfo="updateEmployees($event)"></employee-form-component> -->
    <employees-table-component :employees ="employees" ></employees-table-component>
  </div>
</template>

<script>

import EmployeesTableComponent from './EmployeesTableComponent.vue'
import EmployeeFormComponent from './EmployeeFormComponent.vue'

export default {
  components: { EmployeesTableComponent,  EmployeeFormComponent},
data(){
  return{
    employees: [
      {
        id:1,
        name: "Diganta",
        email: 'blabla@diganta.com'
      },
      {
        id:2,
        name: "Shafi",
        email: 'blabla@shafi.com'
      },
      {
        id:3,
        name: "Mafi",
        email: 'blabla@mafi.com'
      },
      {
        id:4,
        name: "Kufi",
        email: 'blabla@kufi.com'
      },
    ]
  }
  
},
methods:{
  updateEmployees(employee){
    console.log(employee.employeeEmail)
    // console.log('This is Employee Info', employeeInfo.name)
    this.employees = [...this.employees, employee]
    console.log(this.employees)
  }
}
}
</script>

<style>

</style>