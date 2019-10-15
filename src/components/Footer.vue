<template>
  <footer>
    <b-container class="pt-4 pb-3">
      <b-row class="py-2">
        <b-col v-for="title in foots" :key='title.index' >
          <span>{{ title.title }}</span>
            <div v-for="item in title.links" :key='item.index'>
              <b-link :href='item.href' target='_blank' >{{ item.name }}</b-link>
            </div>
        </b-col>
      </b-row>
      <b-row class="py-2">
        <b-col center>
          <b-link :href='copyright.icp.href' target='_blank'>{{ copyright.icp.name }}</b-link> |
          {{ copyright.cn }} <br />
          {{ copyright.en }}
        </b-col>
      </b-row>
    </b-container>
  </footer>
</template>

<script>
export default {
  data () {
    return {
      foots: [
        {
          title: '我的',
          links: [
            {
              name: 'GitHub 主页',
              href: 'https://github.com/Weiyi-C'
            },
            {
              name: 'CSDN 博客',
              href: 'https://blog.csdn.net/u011618035'
            }
          ]
        },
        {
          title: '链接',
          links: [
            {
              name: 'BootstrapVue',
              href: 'https://bootstrap-vue.js.org/'
            }
          ]
        }
      ],
      copyright: {
        icp: {
          name: '蜀ICP备17008351号',
          href: 'http://www.miitbeian.gov.cn/'
        },
        cn: '郑维一 © 版权所有',
        en: 'Copyright © 2019. ZhengWeiyi All rights reserved.'
      }
    }
  }
}
</script>

<style scoped>
a {
  color: #111
}
</style>
