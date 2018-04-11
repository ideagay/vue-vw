<template>
  <div>
    <div class="hello">

    </div>
    <div w-188-246></div>
    <div class="border"></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  .hello{
    width: 400px;
    height: 200px;
    background: red;
  }
  .world{
    background: green;
  }
  [w-188-246] {
    width: 188px;
    height: 246px;
    background-color: green;
  }
  [w-188-246] {
    aspect-ratio: '188:246';
  }
  @svg 1px-border {
    height: 2px;
    @rect {
      fill: var(--color, black);
      width: 100%;
      height: 50%;
    }
  }
  .border {
    height: 30px;
    border: 1px solid transparent;
    border-image: svg(1px-border param(--color #00b1ff)) 2 2 stretch;
  }

</style>
