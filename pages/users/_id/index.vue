<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {

  validate (data) {  // this method will be executed before rendering a route (nuxt.js method)
    return /^\d+$/.test(data.params.id)
  },


  layout: 'users'

}
</script>
