<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-simple-table class="ml-2">
        <tbody>
          <tr v-for="(sale, i) in sales" :key="i">
            <td class="text-center">
              <v-avatar :size="i >= 1 ? 50 : 75" class="align-self-center">
                <v-img
                  src="https://demos.creative-tim.com/material-dashboard-pro/assets/img/faces/avatar.jpg"
                />
              </v-avatar>
            </td>
            <td v-text="sale.salesInM" />
          </tr>
        </tbody>
      </v-simple-table>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  data() {
    return {
      sales: [
        {
          country: 'USA',
          salesInM: 2920
        },
        {
          country: 'Germany',
          salesInM: 1300
        },
        {
          country: 'Australia',
          salesInM: 760
        },
        {
          country: 'United Kingdom',
          salesInM: 690
        },
        {
          country: 'Romania',
          salesInM: 600
        }
      ]
    }
  }
}
</script>
