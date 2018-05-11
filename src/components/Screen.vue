<template>
  <div class="calc-screen">
    <div class="calc-operation">2536 + 419 + </div>
    <div class="calc-typed">2955<transition name="fade"><span v-if="show" class="blink-me" transition="fadeIn">_</span></transition></div>
  </div>
</template>

<script>
export default {
  data : function(){
    return {
        show: true,
        intervalid: null
    }
  },
  mounted: function () {
    this.blink()
  },
  beforeDestroy: function () {
    clearInterval(this.intervalid)
  },
  methods: {
    blink: function () {
      this.intervalid = setInterval(function () {
          this.show = !this.show;
      }.bind(this), 400);
    }
  }
}
</script>

<style>
.calc-screen {
  background: #3A4655;
  width: 100%;
  height: 150px;
  padding: 20px;
}

.calc-operation {
  text-align: right;
  color: #727B86;
  font-size: 21px;
  padding-bottom: 10px;
  border-bottom: dotted 1px;
}

.calc-typed {
  margin-top: 20px;
  font-size: 45px;
  text-align: right;
  color: #fff;
}

.blink-me {
  color: #E0B612;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity .5s;
}

.fade-enter, .fade-leave-to {
  opacity: 0;
}
</style>
