<template>
  <div>
    <div id="home">
      <br /><br /><br />
      <h2>Welcome!</h2>
      <br />
      <p id="intro">
        Feeling bored? Test your luck right here with this literally very random
        game! Good Luck!
      </p>

      <h3>Instructions:</h3>
      <p>
        5 buttons, 10 rounds. Choose within 5 buttons and see if you picked the
        correct button within 10 tries. <br />
        No one really knows which button is THE ONE for each round! Click the
        start button below to play :))
      </p>
      <br />
      <button v-on:click="start()" type="button">Start</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  components: {},
  methods: {
    start() {
      this.$router.push({
        path: "start",
      });
    },
  },
};
</script>

<style scoped>
#home {
  margin: 2em;
  padding-left: 5em;
  padding-top: 1em;
  color: black;
  height: 100%;
}

h2 {
  font-size: 3em;
}

h3 {
  font-size: x-large;
}

#intro {
  color: rgb(107, 107, 107);
}

button {
  background-color: #2e70d3;
  border-color: #2e70d3;
  width: 40%;
  height: 40px;
  float: center;
  right: 10cm;
  max-width: 70%;
  margin: 50px;
  margin-top: 10px;
  padding: 0 5px;
  box-sizing: border-box;
  font-size: 20px;
  border-radius: 10px;
  border-width: 1px;
  font-family: "Trebuchet MS", "Lucida Sans Unicode", "Lucida Grande",
    "Lucida Sans", Arial, sans-serif;
  font-style: italic;
}

button:hover {
  border: 2px solid #90caf9;
  background-color: #90caf9;
  color: white;
  cursor: pointer;
}

p {
  font-size: 20px;
  /*font-family: "Arial";*/
}

img {
  width: 100%;
  height: 700px;
}

#foot {
  background-color: #faedcd;
}
</style>
