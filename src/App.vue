<template>
  <div id="app">
    <div class="container">
      <div class="calc-body">
        <Screen></Screen>
        <Key></Key>
      </div>
    </div>
  </div>
</template>

<script>
import Screen from './components/Screen';
import Key from './components/Key';

export default {
  name: 'app',
  components: {
    Screen,
    Key
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
}

body {
  background: #EAEBEC;
}

.container {
  width: 400px;
  height: 100%;
  margin: 20% auto;
}

.calc-body {
  width: 400px;
  margin: auto;
  min-height: 400px;
  border: solid 1px #3A4655;
  box-shadow: 0 8px 50px -7px black;
}
</style>
