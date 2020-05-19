<template>
  <div class="home">
    <el-input v-model="input" placeholder="请输入搜索内容"></el-input>
    <el-button type="primary" @click="doSearch">搜索</el-button>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      input: ''
    }
  },
  methods: {
    doSearch(e) {
      console.log('click', e);
      this.$router.push({path:'/search',query:{key:this.input}});
    }
  }
}
</script>
