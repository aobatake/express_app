<template>
  <div id="nav">
    <ul>
      <li class="left-nav"><a href="/">Home</a></li>
      <li><a href="/reddit">Reddit</a></li>
      <li><a href="#">Twitter</a></li>
      <li class="right-nav"><a href="#">Sign In</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'navbar',
};

</script>

<style lang="scss" scoped>

#nav {
  background: #FFF;
  margin-bottom: 40px;
}

ul {
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
  height: 50px;
  margin: 0;
}

li {
  display: inline-block;
  list-style: none;
  margin: 0;
}

a {
  box-sizing: border-box;
  color: #000;
  display: block;
  float: left;
  height: 50px;
  padding: 1em;
  text-decoration: none;
  &:hover {
    border-bottom: 5px solid rgba(85,158,131,1);
  }
}

.left-nav {
  margin-left: 40px;
}

.right-nav {
  float: right;
  margin-right: 40px;
}


</style>
