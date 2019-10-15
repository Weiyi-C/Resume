<template>
  <footer>
    <b-container>
      <b-row>
        <b-col v-for="title in foots" :key='title.index' >
          <span>{{ title.title }}</span>
          <ul>
            <li v-for="item in title.links" :key='item.index'>
              <b-link :href='item.href' target='_blank' >{{ item.name }}</b-link>
            </li>
          </ul>
        </b-col>
      </b-row>
      <b-row>
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
          title: '友情链接',
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
        }
      ],
      copyright: {
        icp: {
          name: '蜀ICP备17008351号',
          href: 'http://www.miitbeian.gov.cn/'
        },
        cn: '郑维一 © 版权所有',
        en: 'Copyright © 2017-2019. ZhengWeiyi All rights reserved.'
      }
    }
  }
}
</script>
