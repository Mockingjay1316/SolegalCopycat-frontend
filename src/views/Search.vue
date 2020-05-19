<template>
  <div class="about">
    <h1>{{ this.$route.query.id }}</h1>
  </div>
</template>

<script>
export default {
  name: 'Search',
  mounted: function () {
    console.log('get ' + this.$route.query.id)
  }
}
</script>