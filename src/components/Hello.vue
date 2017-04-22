<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <ul>
      <li>
        1、px 做了 rem 转换
      </li>
      <li>
        2、字体做了 dpr 适配，可以用 chrome 模拟 ip5、ip6、plus 看看
      </li>
    </ul>
    <div class="for-app">
      我的样式来自于全局的 app.scss 文件
    </div>
  </div>

</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style scoped>
  h1
  {
    font-size: 24px;
    line-height: 120px;
    text-align: center;
  }

</style>


<style lang="scss" scoped>
  ul {
    margin: 10px;
    padding: 30px 10px;
    border: solid 1px #ccc;
    background-color: #fff;
  }

  li {
    font-size: 16px;
    line-height: 50px;
    text-align: left;
  }

  li + li
  {
    margin-top: 20px;
  }
</style>
