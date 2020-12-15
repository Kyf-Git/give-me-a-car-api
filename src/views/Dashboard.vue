<template>
  <table id="stock">
    <thead>
      <tr>
        <th>ID</th>
        <th>Marque</th>
        <th>Km</th>
        <th>Disponibilité</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="row in rows" v-bind:key="row" v-bind:row="row">
        <td>{{ row.id }}</td>
        <td>{{ row.marque }}</td>
        <td>{{ row.km }}</td>
        <td>{{ row.disponibilité }}</td>
      </tr>
    </tbody>
  </table>
</template>

<style>
#stock {
  margin-left: auto;
  margin-right: auto;
}

table {
  font-family: "Open Sans", sans-serif;
  width: 750px;
  border-collapse: collapse;
  border: 3px solid #44475c;
  margin: 10px 10px 0 10px;
}

table th {
  text-transform: uppercase;
  text-align: left;
  background: #44475c;
  color: #fff;
  padding: 8px;
  min-width: 30px;
}

table td {
  text-align: left;
  padding: 8px;
  border-right: 2px solid #7d82a8;
}
table td:last-child {
  border-right: none;
}
table tbody tr:nth-child(2n) td {
  background: #d4d8f9;
}
</style>

<script>
export default {
  name: "Dashboard",
  data() {
    return {
      rows: [
        { id: 1, marque: "Renault", km: 25300, disponibilité: true },
        { id: 2, marque: "Peugeot", km: 37853, disponibilité: true },
        { id: 3, marque: "Fiat", km: 62872, disponibilité: true },
        { id: 4, marque: "BMW", km: 125459, disponibilité: true },
        { id: 5, marque: "Citroen", km: 43982, disponibilité: true },
      ],
    };
  },
};
</script>

