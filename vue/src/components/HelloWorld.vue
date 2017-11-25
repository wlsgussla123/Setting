<template>
  <div>
    <div class="hello">
      <h1>{{ msg }}</h1>
    </div>

    <div :class="$style.test"> 
      <span :id="$style.text">scss 적용</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" module>
h1 {
  font-weight: normal;
}

.test {
  #text {
    color: red;
  }
}

</style>
