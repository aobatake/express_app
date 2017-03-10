<template>
  <div id="clock">
    <h2>Today is {{ date }}</h2>
    <h2>The time is {{ time }}</h2>
  </div>
</template>

<script>
const moment = require('moment');

export default {
  name: 'clock',
  data() {
    return {
      time: '',
      date: '',
    };
  },
  methods: {
    getDate() {
      this.date = moment().format('MMMM Do YYYY');
    },
    getTime() {
      this.time = moment().format('h:mm:ss a');
    },
  },
  mounted() {
    this.getDate();
    this.getTime();
    setInterval(() => {
      this.getDate();
      this.getTime();
    }, 1000);
  },
};

</script>

<style lang="scss" scoped>
  #clock {
    margin-left: 40px;
  }

</style>
