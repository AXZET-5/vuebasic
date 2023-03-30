<template>
  <div id="app">
    <h1 id="toChange">Sticker Generator</h1>
    <div class="ContainingBox">
      <h1>Hi</h1>
    </div>
    <br>
    <p>Click any of these buttons to generate the corresponding sticker!</p>
    <button @click="switchTo(1)" type="button">1</button>
    <button @click="switchTo(2)" type="button">2</button>
    <button @click="switchTo(3)" type="button">3</button>
    <button @click="switchTo(4)" type="button">4</button>
    <button @click="switchTo(5)" type="button">5</button>
  </div>
</template>



<script>
  export default {
    methods: {
      switchTo(number) {
        var text = document.getElementById('toChange');

        text.innerHTML(String(number));
      }
    }
  }
</script>



<style>

body {
  background-color: rgb(0,0,30);
  text-align: center;
}

.ContainingBox {
  border: 3px solid white;
  width: fit-content;
  margin-left: auto;
  margin-right: auto;
  padding: 20px;
  border-radius: 50px;
}

h1 {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 50px;
  color: white;
}

p {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 20px;
  color: white;
}

img {
  width: 300px;
}

button {
  padding-top: 10px;
  padding-bottom: 10px;
  padding-left: 20px;
  padding-right: 20px;
  margin-left: 10px;
  margin-right: 10px;
  margin-bottom: 10px;

  font-family: Arial, Helvetica, sans-serif;
  font-size: 20px;
  font-weight: bold;
  color: rgb(0,0,30);
  border-radius: 50px;
  border: 3px solid white;

  transition-duration: 0.2s;
}

button:hover {
  scale: 1.20;
  cursor: pointer;
  background-color: lime;
}

button:focus {
  scale: 1.50;
  background-color: yellow;
}

</style>
