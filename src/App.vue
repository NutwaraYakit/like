<template>
  <div id="app">
    <header>
      <img src="./assets/bg.jpg" width="100%" />
      <img class="rounded-circle" src="./assets/avatar.jpg" width="15%" />
    </header>
    <br />
    <HelloWorld msg=" Nature" />
    <p>The best gift is to see myself happy.</p>
    <br />
    <br />
    <hr />
    <ul>
      <ul>
        <button id="hh">
          <img id="imghh" src="./assets/home-run.png" />
        </button>
        <button id="ms">
          <img id="imgms" src="./assets/telegram.png" />
        </button>
        <button id="pp">
          <img id="imgpp" src="./assets/user.png" />
        </button>
      </ul>
    </ul>
    <hr />
    <br />
    <br />

    <br />
    <div class="row">
      <div class="col">
        <img class="rounded border border-white" src="./assets/img1.jpg" width="60%" />
        <br />
        <br />
        <coun />
        <br />
        <br />
        <hr />
        <br />
      </div>
    </div>
    <div class="row">
      <div class="col">
        <img class="rounded border border-white" src="./assets/img2.jpg" width="60%" />
        <br />
        <br />
        <coun />
        <br />
        <br />
        <hr />
        <br />
      </div>
    </div>
    <div class="row">
      <div class="col">
        <img class="rounded border border-white" src="./assets/img3.jpg" width="60%" />
        <br />
        <br />
        <coun />
        <br />
        <br />
        <hr />
        <br />
      </div>
    </div>
    <div class="row">
      <div class="col">
        <img class="rounded border border-white" src="./assets/img4.jpg" width="60%" />
        <br />
        <br />
        <coun />
        <br />
        <br />
        <hr />
        <br />
      </div>
    </div>
    <br />
    <hr />
    <br />
    <br />
    <br />
    <div class="row">
      <br />
      <hr />
      <br />
      <br />
      <br />
      <br />
      <br />
      <div class="col">
        <fonts />
        <hr />
        <div class="row-12">
          Name
          <input id="box" type="text" v-model="name" />
          <br />
          <br />
          No...
          <input id="box" type="text" v-model="code" />
          <br />
          <br />
        </div>
        <p>Output</p>
        <button id="coww">
          <div class="row-12">ชื่อ {{name}}</div>
          <div class="row-12">รหัสนักศึกษา {{code}}</div>
        </button>
        <br />
        <br />
        <br />
      </div>
    </div>
    <footer class="my-5 pt-5 text-muted text-center text-small">
      <p class="mb-1">&copy; cs313@6104101346</p>
    </footer>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import coun from "./components/like.vue";
import fonts from "./components/fonts.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    coun,
    fonts,
  },
  data: function () {
    return {
      total: 0,
      name: "",
      code: "",
      gpa: 0.1,
    };
  },
};
</script>




<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #241602;
  margin-top: 50px;
}
#ul {
  display: inline;
  padding: 70px;
  widows: 0px;
  font-size: 50px;
  font-weight: bold;
}
#hh {
  border-radius: 30px;
  width: 250px;
  height: 50px;
  background-color: white;
  border: 2px solid #ffffff;
}
#imghh {
  width: 35px;
}
#ms {
  border-radius: 30px;
  width: 250px;
  height: 50px;
  background-color: white;
  border: 2px solid #ffffff;
}
#imgms {
  width: 35px;
}
#pp {
  border-radius: 30px;
  width: 250px;
  height: 50px;
  background-color: white;
  border: 2px solid #ffffff;
}
#imgpp {
  width: 35px;
}
#box {
  border-radius: 30px;
  width: 350px;
  height: 40px;
  background-color: white;
  border: 2px solid #4aa7cc;
}
#coww {
  border-radius: 40px;
  width: 500px;
  height: 100px;
  background-color: white;
  border: 2px solid #747474;
}
</style>
