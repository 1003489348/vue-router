 <template>
  <div id="app">
    <div id="nav">
      <div id="nav2"><img src="./logo.png"></div>
      <div id="nav1"><router-link to="/">Home</router-link></div>
      <div id="nav1"><router-link to="/about">About</router-link></div>
      <div id="nav1"><router-link to="/chat">Chat</router-link></div>
    </div>
    <router-view/>
    <my></my>
  </div>
</template>

<script>
import my from "./child";
export default {
  data(){
   
  },
  components:{
    my:my
  }

}
</script>


<style lang="scss">
*{
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  background: rgb(214, 166, 8);
  height: 100px;
  line-height: 100px;
}
#nav1{
  background:rgb(214, 166, 8);
  width:25%;
  height: 100px;
  float:left;
  position: relative;
}
#nav router-link{
  display: block;
  background:rgb(214, 166, 8);
}
#nav2{
  background:rgb(84, 216, 198);
  width:25%;
  height: 100px;
  float:left;
  color: #000000;
  font-size: 24px;
  }
#nav2 img{
  width: 50px;
  height: 50px;
  margin-top: 25px;
}
#nav a {
    text-decoration: none;
    font-weight: bold;
    color: #000000;
    &.router-link-exact-active {
      color: #fafafa;
    }
  }
#footer{
  width: 100%;
  height: 100px;
  background: #000000;
  color: #fafafa;
  line-height: 100px;
}
</style>
