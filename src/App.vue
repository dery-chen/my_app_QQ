<template>
  <div id="app">
    <div id="nav">
    <span></span>
     <span>消息</span>
    <span>+</span>
    </div>
    <router-view/>
    <footer>
     <router-link to="/home">消息</router-link>
     <router-link to="/persons">联系人</router-link>
     <router-link to="/state">动态</router-link>
    </footer>
  </div>
</template>

<style lang="scss">
// #app {
//   font-family: 'Avenir', Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
// }

// #nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
</style>
