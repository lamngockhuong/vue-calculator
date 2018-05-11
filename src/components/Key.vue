<template>
  <div class="key">
      <div class="calc-button-row">
        <div class="button c">C</div>
        <div class="button l">≠</div>
        <div class="button l">%</div>
        <div class="button l">/</div>
      </div>
      <div class="calc-button-row">
        <div class="button">7</div>
        <div class="button">8</div>
        <div class="button">9</div>
        <div class="button">%</div>
        <div class="button">&#8617;</div>
        <div class="button">#</div>
      </div>
      <div class="calc-button-row">
        <div class="button">4</div>
        <div class="button">5</div>
        <div class="button">6</div>
        <div class="button l">−</div>
      </div>
      <div class="calc-button-row">
        <div class="button">1</div>
        <div class="button">2</div>
        <div class="button">3</div>
        <div class="button l">+</div>
      </div>
      <div class="calc-button-row">
        <div class="button">.</div>
        <div class="button">0</div>
        <div class="button">&lt;</div>
        <div class="button l">=</div>
      </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.key {
  height: 300px;
}

.calc-button-row {
  width: 100%;
  background: #3c4857;
}

.button {
  width: 100/6%;
  background: #425062;
  color: #fff;
  padding: 20px;
  display: inline-block;
  font-size: 25px;
  text-align: center;
  vertical-align: middle;
  margin-right: -4px;
  border-right: solid 2px #3c4857;
  border-bottom: solid 2px #3c4857;
  transition: all 0.2s ease-in-out;
}

.button.l {
  color: #aeb3ba;
  background: #404d5e;
}

.button.c {
  color: #d95d4e;
  background: #404d5e;
}

.button:hover {
  background: #e0b612;
  transform: rotate(5deg);
}

.button.c:hover,
.button.l:hover {
  background: #e0b612;
  color: #fff;
}
</style>
