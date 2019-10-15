<template>
  <b-container class="my-4">
    <b-row class="py-5 row">
      <b-col>
        <b-img-lazy center fluid :src=photoSrc alt="郑维一的照片">郑维一的照片</b-img-lazy>
      </b-col>
      <b-col>
        <table class="table table-striped">
          <tbody>
            <tr>
              <td>姓&#12288;名</td>
              <td colspan="3">郑维一</td>
            </tr>
            <tr>
              <td>性&#12288;别</td>
              <td>男</td>
              <td>出&#12288;生</td>
              <td>1997年2月1日</td>
            </tr>
            <tr>
              <td>名&#12288;族</td>
              <td>汉族</td>
              <td>籍&#12288;贯</td>
              <td>四川省成都市</td>
            </tr>
            <tr>
              <td>身&#12288;高</td>
              <td>180cm</td>
              <td>体&#12288;重</td>
              <td>65kg</td>
            </tr>
            <tr>
              <td>电&#12288;话</td>
              <td><a href="tel:13568810905">13568810905</a></td>
              <td>Ｑ&#12288;Ｑ</td>
              <td><a target="_blank" href="http://wpa.qq.com/msgrd?v=3&uin=549307315&site=qq&menu=yes">549307315</a></td>
            </tr>
            <tr>
              <td>E-mail</td>
              <td>weiyi@zhengweiyi.cn</td>
              <td>微&#12288;博</td>
              <td>@曦璞维一</td>
            </tr>
            <tr>
              <td>通&#12288;信</td>
              <td colspan="3">四川省成都市金堂县清平街68号</td>
            </tr>
            <tr>
              <td>学&#12288;校</td>
              <td>四川大学锦城学院</td>
              <td>专&#12288;业</td>
              <td>移动应用开发</td>
            </tr>
          </tbody>
        </table>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  data () {
    return {
      photoSrc: require('../assets/photo.jpg')
    }
  }
}
</script>

<style scoped>
.row {
  background: #FFF;
  box-shadow: 0 0 5 2 rgba(0,0,0,0.4)
}
</style>
