<template>
  <Sidebar />
  <div>
    <Employee />
  </div>
  <div id="schedule-and-header">
    <Header />
    <EmployeeShifts />
  </div>


</template>


<script setup>
import Sidebar from "./components/Sidebar.vue";
import Employee from "./components/Employee.vue";
import EmployeeShifts from "./components/EmployeeShifts.vue";
import Header from "./components/Header.vue";
</script>

<style>
body {
  margin: 0;
  font-family: PolySans Trial;
}

header {
  margin-bottom: 3rem;
}
</style>
