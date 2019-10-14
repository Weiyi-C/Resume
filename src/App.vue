<template>
  <div>
    <div class="nav">
      <nav>
        <div>
          <ul>
            <li v-for='item in nav' :key='item'>{{ item.name }}</li>
          </ul>
        </div>
      </nav>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      nav: [
        { name: '返回首页', url: '' },
        { name: '基本信息', url: '' },
        { name: 'Web', url: '' },
        { name: '移动', url: '' },
        { name: '设计', url: '' }
      ]
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  line-height: 2rem;
}

body {
  margin: 0;
  font-size: 16px;
  font-family: "Microsoft YaHei";
  background-color: #FEFEFE;
}

.nav {
  position: flxed;
  top: 0px;
  left: 0px;
  width: 100%;
  overflow: hidden;
  background-color: #FFF;
  box-shadow: 0px -2px 20px 3px rgba(0,0,0,0.2);
}

.nav nav {
  margin: 0 auto;
  width: 1180px
}

.nav ul {
  float: right;
  list-style-type: none;
}

.nav ul li {
  float: left;
  padding: 0 2rem;
  line-height: 5;
}

.row {
  padding: 20px 0;
}
</style>
