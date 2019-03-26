# vue-axios


## install:
cnpm install --save axios vue-axios

## entry file
import Vue from 'vue'

import axios from 'axios'

import VueAxios from 'vue-axios'


Vue.use(VueAxios, axios)

## Usage
Vue.axios.get(api).then((response) => {
  console.log(response.data)
})

this.axios.get(api).then((response) => {
  console.log(response.data)
})

this.$http.get(api).then((response) => {
  console.log(response.data)
})

## vue官方实例：
this.axios
      .get('https://api.coindesk.com/v1/bpi/currentprice.json')
      .then(response => {
        this.info = response.data.bpi
      })
      .catch(error => {
        console.log(error)
        this.errored = true
      })
      .finally(() => this.loading = false)
