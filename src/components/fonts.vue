<template>
  <div>
    <p v-bind:style="{ fontSize: fsize + 'px' }" class="text-info">Infomation</p>
    <li>
      <button @click="upFunction" id="up">+</button>
    </li>
    <li>
      <button @click="downFunction" id="down">-</button>
    </li>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      counter: 0,
      fsize: 50,
    };
  },
  props: {
    lable: String,
  },
  methods: {
    upFunction: function () {
      this.fsize += 10;
      console.log("fsize = " + this.fsize);
    },
    downFunction: function () {
      this.fsize -= 10;
      console.log(this.fsize);
    },
  },
};
</script> 
<style>
li {
  display: inline;
  padding: 10px;
  widows: 0px;
  font-size: 15px;
  font-weight: bold;
}
#up {
  border-radius: 30px;
  width: 40px;
  height: 40px;
  font-size: 30px;
  background-color: rgb(255, 255, 255);
  border: 2px solid #ffffff;
  color: rgb(23, 118, 182);
}
#down {
  border-radius: 30px;
  width: 40px;
  height: 40px;
  font-size: 35px;
  background-color: rgb(255, 255, 255);
  border: 2px solid #ffffff;
  color: rgb(23, 118, 182);
}
</style>