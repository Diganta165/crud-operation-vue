<template>
  <div>
      <h1>This is Employees Table</h1>
      <table>
          <tr>
              <th>Id</th>
              <th>Name</th>
              <th>Email</th>
          </tr>
          <tr v-for="employee in employees" :key="employee.id">
              <td>{{employee.id}}</td>
              <td>{{employee.name}}</td>
              <td>{{employee.email}}</td>
          </tr>
      </table>
  </div>
</template>

<script>
export default {
    props:{
        employees: Array
    }
}
</script>

<style>

</style>