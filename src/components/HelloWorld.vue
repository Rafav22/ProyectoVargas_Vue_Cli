<template>
  <table :style="{ color: textColor, background: backgroundColor }">
    <thead>
      <tr>
        <th>Nombre</th>
        <th>Edad</th>
        <th>Email</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(item, index) in data" :key="index">
        <td>{{ item.nombre }}</td>
        <td>{{ item.edad }}</td>
        <td>{{ item.email }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  props: {
    data: {
      type: Array,
      required: true
    },
    textColor: {
      type: String,
      default: 'black'
    },
    backgroundColor: {
      type: String,
      default: 'white'
    }
  }
}
</script>

<style scoped>
table {
  
  width: 0;
  border-collapse: collapse;
}

th, td {
  padding: 8px;
  border-bottom: 1px solid #ddd;
}

th {
  text-align: left;
}

tr:nth-child(even) {
  background-color: #4f56d4;
}
</style>
