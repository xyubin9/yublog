<template>
  
  <div id="app">
    <!-- 流光背景 -->
    <div class="background">
        <canvas id="startrack"></canvas>
        <div class="cover"></div>
    </div>
    <!-- 导航列表 -->
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
      <a href="http://api.wqwlkj.cn/wqwlapi/qq_friend.php?qq=983847647">QQ</a>
    </nav>
    <!-- 音乐播放器 -->
    <audio autoplay>
      <source src="https://api.uomg.com/api/rand.music?sort=热歌榜" type="audio/mpeg">
    </audio>
    
    <router-view/>
   
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50; */
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
