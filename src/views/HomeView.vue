<template>
  <div class="home">
    <table width="100%">
      <thead>
          <tr>
              <th scope="col">Турниры</th>
              <th scope="col">Название</th>
              <th scope="col">Дата начала</th>
              <th scope="col">Дата окончания</th>
          </tr>
      </thead>
      <tbody>
          <tr v-for="i in react" :key="i.name">
            <td>
              <img height="100" :src="i.logo" />
            </td>
            <td>
              {{i.name}}
            </td>
            <td>
              {{i.date_from}}
            </td>
            <td>
              {{i.date_to}}
            </td>

          </tr>
      </tbody>
  </table>
  </div>
</template>

<script>
import s from "../../event"
export default {
  name: 'HomeView',
  data() {
    return {
      react: s
    }
  }
}
</script>
   