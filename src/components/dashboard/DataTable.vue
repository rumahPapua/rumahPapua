<template>
  <div class="container">
    <h3>Data Penerima Beasiswa</h3>
    <table>
      <thead>
        <tr>
          <th>Nama</th>
          <th>TTL</th>
          <th>Pekerjaan</th>
          <th>Status pekerjaan</th>
          <th>Pendidikan</th>
          <th>Pemberi Beasiswa</th>
          <th>Jumlah Beasiswa</th>
        </tr>
      </thead>
      <tbody>
        <!-- <tr v-for="student in students">
          <td>{{ student.fullname }}</td>
          <td>{{ student.birthdate }}</td>
          <td>{{ student.occupation }}</td>
          <td>{{ student.working_status }}</td>
          <td>{{ student.education }}</td>
          <td>{{ student.scholarship_provider }}</td>
          <td>{{ student.amount_scholarship }}</td>
        </tr> -->
        <tr v-bind:key="data in datas">
          <td>{{ data.first_name }} {{ data.last_name }}</td>
          <td>{{ data.date_birth }}</td>
          <td>{{ data.occupation }}</td>
          <td>{{ data.working_status[Math.floor(Math.random() * Math.floor(3))] }}</td>
          <td>{{ data.education }}</td>
          <td>{{ data.scholarship_provider }}</td>
          <td>Rp {{ (data.amount_scholarship).toFixed(2).replace(/\d(?=(\d{3})+\.)/g, '$&,') }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
import dataJson from '../../utils/MOCK_DATA.json'
export default {
  components: {
    // DataTable
  },
  data () {
    return {
      students: [
        {
          fullname: 'Neas Wanimbo',
          birthdate: '20 July 1995',
          occupation: 'student, motivator',
          working_status: 'scholarship grantee',
          education: 'Tanri Abeng University',
          scholarship_provider: 'PT Freeport',
          amount_scholarship: '20000000'
        }
      ],
      datas: dataJson
    }
  }
}
</script>

<style>

table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

td, th {
  border: 2px solid #dddddd;
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #1dece2;
}
</style>
