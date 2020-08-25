<template>
  <div>
    <div class="row-12">
      <button @click="like()" class="btn-outline-info">
        <i class="fa fa-thumbs-o-up" aria-hidden="true"></i> Like
      </button>
      <button @click="love()" class="btn-outline-info">
        <i class="fa fa-thumbs-o-up" aria-hidden="true"></i> Love
      </button>
      <button @click="comic()" class="btn-outline-info">
        Comic
        <i class="fa fa-thumbs-o-up" aria-hidden="true"></i>
      </button>
      <button @click="wow()" class="btn-outline-info">
        Wow
        <i class="fa fa-thumbs-o-up" aria-hidden="true"></i>
      </button>
      <button @click="sad()" class="btn-outline-info">
        Sad
        <i class="fa fa-thumbs-o-down" aria-hidden="true"></i>
      </button>
      <button @click="angry()" class="btn-outline-info">
        <i class="fa fa-thumbs-o-down" aria-hidden="true"></i> Angry
      </button>
      <button @click="reset()" class="btn-outline-info">
        <i class="fa fa-refresh" aria-hidden="true"></i> reset
      </button>
      <br />
      <br />
      <button id="cc">
        <p v-bind:style="{fontSize: fonts + 'px' }">
          <i id="fcc">{{ counter }}</i>
        </p>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      counter: 0,
      fonts: 50,
    };
  },
  methods: {
    Like: function () {
      this.counter += 1;
      console.log(this.counter);
    },
    Love: function () {
      this.counter += 10;
      console.log(this.counter);
    },
    comic: function () {
      this.counter += 5;
      console.log(this.counter);
    },
    wow: function () {
      this.counter += 20;
      console.log(this.counter);
    },
    Sad: function () {
      this.counter -= 5;
      console.log(this.counter);
    },
    angry: function () {
      this.counter -= 50;
      console.log(this.counter);
    },
    reset: function () {
      this.counter = 0;
      console.log(this.counter);
    },
  },
};
</script>


<style>
#cc {
  border-radius: 40px;
  width: 200px;
  height: 70px;
  background-color: white;
  border: 2px solid #cacaca;
}
#fcc {
  font-size: 25px;
  color: #9e9e9e;
}
.btn-outline-info {
  border-radius: 50px;
  width: 90px;
  height: 50px;
  border: 2px solid #000000;
  background-color: #000000;
  color: white;
}
</style>