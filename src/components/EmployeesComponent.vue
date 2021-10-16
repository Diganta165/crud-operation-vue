<template>
  <div>
    <h1>This is Employees Component</h1>
    <employees-table-component :employees ="employees"></employees-table-component>
  </div>
</template>

<script>

import EmployeesTableComponent from './EmployeesTableComponent.vue'

export default {
  components: { EmployeesTableComponent },
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
  
}
}
</script>

<style>

</style>