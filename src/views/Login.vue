<template>
  <v-card class="d-flex flex-row justify-center mt-12" flat tile>
    <v-card class="d-lg-6 d-sm-12 px-5" raised shaped>
      <v-card-title>Scan QR to Login</v-card-title>
      <v-img class="mb-4" src="https://i.loli.net/2020/06/12/Lazfdiuc6QrA82J.png" max-width="200"></v-img>
    </v-card>
  </v-card>
</template>

<script>
import axios from 'axios'

export default {
  name: 'Login',
  mounted() {
    (async () => {
      const { data: { data: { isLogin } } } =  await axios.get('/qrcode/status')
      if (isLogin) {
        console.log(123)
        this.$router.push('bucket')
      }
    })()
  },
  data() {
    return {
      isLogin: false
    }
  }
}
</script>
