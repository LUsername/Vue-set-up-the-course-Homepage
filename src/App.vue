<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
*{
  padding: 0;
  margin: 0;
  list-style: none;
}
/* 去除router-link默认样式 */
a{
  text-decoration: none;
}
</style>
