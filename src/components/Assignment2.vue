<template>
  <div id="exercise">
    <!-- 1) Show an alert when the Button gets clicked -->
    <div>
        <button v-on:click="onClick">Show Alert</button>
    </div>
    <!-- 2) Listen to the "keydown" event and store the value in a data property (hint: event.target.value gives you the value) -->
    <div>
        <input v-on:keyup="onKeyUp" type="text" />
        <p>{{ inputVal }}</p>
    </div>
    <!-- 3) Adjust the example from 2) to only fire if the "key down" is the ENTER key -->
    <div>
        <input v-on:keydown.enter="onKeyDownEnter" type="text" />
        <p>{{ input2Val }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Assignment2',
  data () {
    return {
      inputVal: '',
      input2Val: ''
    }
  },
  methods: {
    onClick: function () {
      alert('Button was clicked!')
    },
    onKeyUp: function (event) {
      this.inputVal = event.target.value
    },
    onKeyDownEnter: function (event) {
      this.input2Val = event.target.value
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
