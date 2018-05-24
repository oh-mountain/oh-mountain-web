<template>
  <div>
    <header class="header">
      <div class="mr-16">
        <a href="#info" data-scroll><span class="mr-16">INFO</span></a>
        <a href="#about" data-scroll><span class="mr-16">ABOUT</span></a>
        <a href="#dj" data-scroll><span class="mr-16">DJ</span></a>
        <a href="#timetable" data-scroll><span class="mr-16">TIME TABLE</span></a>
        <a href="#access" data-scroll><span>ACCESS</span></a>
      </div>
    </header>
    <div class="contents">
      <section class="top">
        <div style="width: 760px;margin: auto;">
          <img src="../../assets/img/mountain20180421.png" alt="Oh!Mountain 2018/07/07" width="100%">
        </div>
      </section>
      <section id="info" class="info">
        <div class="contents">
          <h1 class="mb-16">
            Oh!Mountain
          </h1>
          <p class="mb-24">
            <span class="fs-30 mr-4">2018.04.21 SAT</span>Start:16:00<br/>
            <span class="f-bold">@<a href="http://arena.nomouze.jp/">ARENA下北沢</a></span><br/>
            <span class="fs-16">Entrance Free</span>
          </p>
          <p class="fs-14 mb-8">
            MinimalからDiscoまで、イーブンキックのJourneyを演出、音好きのためのGrooveを作り上げて行くパーティです。今回よりサウンドシステム強化する予定。踊ってよし飲んでよし食べてよし。入場は無料なので皆様奮ってご参加ください。
          </p>
        </div>
      </section>
      <section id="about" class="about">
        <h1 class="mb-16">
          About Oh!Mountain
        </h1>
        <p>
          2015年2月よりアウトドア好きのDJたちによりスタートしたFreakyなミュージックパーティ。音好きのためのHouse/Techno/Discoなどダンスミュージックを幅広く鳴らす。
        </p>
      </section>

      <section id="dj" class="dj">
        <h1 class="mb-16">
          DJ
        </h1>
        <p class="fs-24 mb-8">
          dot nine<br>
          ANNO<br>
          YMD<br>
          DJ Minato<br>
        </p>
      </section>

      <section id="timetable" class="timetable">
        <h1 class="mb-16">
          TimeTable
        </h1>
        <p>
          TBA
        </p>
      </section>

      <section id="access" class="access">
        <div>
          <div id="map_canvas" style="width:100%;height:400px;"/>
        </div>
        <h1 class="balloon">
          ACCESS
        </h1>
      </section>

      <footer class="footer">
        more Infomation → <a href="https://www.facebook.com/events/107512200032002/" target="_blank">Facebook</a>
      </footer>
      <!--<script>-->
      <!--function initialize() {-->
      <!--var latlng = new google.maps.LatLng(35.659691, 139.668556);-->
      <!--var centeratlng = new google.maps.LatLng(35.661047, 139.667043);-->
      <!--var marker = new google.maps.Marker({-->
      <!--position : latlng,-->
      <!--map      : map,-->
      <!--title    : 'ARENA下北沢'-->
      <!--});-->
      <!--var myOptions = {-->
      <!--zoom           : 17, /*拡大比率*/-->
      <!--center         : latlng, /*表示枠内の中心点*/-->
      <!--mapTypeId      : google.maps.MapTypeId.ROADMAP, /*表示タイプの指定*/-->
      <!--scrollwheel    : false,-->
      <!--mapTypeControl : false-->
      <!--};-->
      <!--var map = new google.maps.Map(document.getElementById('map_canvas'), myOptions);-->
      <!--marker.setMap(map);-->
      <!--map.setCenter(centeratlng);-->
      <!--}-->
      <!--</script>-->
      <!--<script>-->
      <!--// スムーススクロールを起動する-->
      <!--smoothScroll.init({offset : '36px'});-->
      <!--</script>-->
    </div>
  </div>
</template>

<script>
export default {
  name: 'TopPc'
}
</script>
<style>
  html,
  body {
    height: 100%;
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    font-size: 100%;
  }

  html,
  body {
    height: 100%;
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    font-size: 100%;
  }

  a {
    text-decoration: none;
    -webkit-transition: all .3s;
    transition: all .3s;
  }

  a:link {
    color: #ffffff;
  }

  a:hover {
    color: #ffffff;
    opacity: 0.5;
  }

  a:visited {
    color: #ffffff;
  }

  ul {
    margin: 0;
    padding: 0;
    list-style-type: none;
  }

  h1,
  p {
    margin: 0;
  }

  h1 {
    font-size: 48px;
  }

  header {
    position: fixed;
    top: 0px;
    width: 100%;
    height: 36px;
    line-height: 36px;
    text-align: right;
    color: #fff;
    background-color: rgba(0, 0, 0, 0.7);
  }

  .header a {
    color: #ffffff;
    text-decoration: none;
  }

  .contents {
    min-width: 760px;
  }

  section {
    min-width: 320px;
    padding: 24px;
  }

  .top {
    margin-top: 36px;
    padding: 0;
    background-color: #f6f7f9;
  }

  .info a {
    color: #ff0000;
    text-decoration: none;
  }

  .event {
    background-color: #ff0000;
  }

  .about {
    background-color: #f6f7f9;
  }

  .access {
    position: relative;
    padding: 0;
  }

  .timetable {
    background-color: #f6f7f9;
  }

  .access .balloon {
    position: absolute;
    top: 20px;
    left: 20px;
    padding: 16px;
    background: #fff;
  }

  footer {
    height: 72px;
    line-height: 72px;
    text-align: center;
  }

  .footer a {
    color: #ff0000;
    text-decoration: none;
  }

  /**
* utils
*/

  /**
  * font
  */

  .fs-10 {
    font-size: 10px !important;
  }

  .fs-12 {
    font-size: 12px !important;
  }

  .fs-14 {
    font-size: 14px !important;
  }

  .fs-16 {
    font-size: 16px !important;
  }

  .fs-18 {
    font-size: 18px !important;
  }

  .fs-20 {
    font-size: 20px !important;
  }

  .fs-22 {
    font-size: 22px !important;
  }

  .fs-24 {
    font-size: 24px !important;
  }

  .fs-30 {
    font-size: 30px !important;
  }

  /**
  * color
  */

  .cl-white {
    color: #fff;
  }

  .cl-black {
    color: #333;
  }

  .cl-light_black {
    color: #555;
  }

  .cl-gray {
    color: #757575;
  }

  .cl-deep_gray {
    color: #555;
  }

  .cl-light_gray {
    color: #b3b3b3;
  }

  .cl-blue {
    color: #063e90;
  }

  .cl-red {
    color: #d43c3c;
  }

  /**
  * margin
  */

  .mt-40 {
    margin-top: 40px !important;
  }

  .mb-2 {
    margin-bottom: 2px !important;
  }

  .mb-4 {
    margin-bottom: 4px !important;
  }

  .mb-8 {
    margin-bottom: 8px !important;
  }

  .mb-10 {
    margin-bottom: 8px !important;
  }

  .mb-12 {
    margin-bottom: 12px !important;
  }

  .mb-16 {
    margin-bottom: 16px !important;
  }

  .mb-18 {
    margin-bottom: 18px !important;
  }

  .mb-20 {
    margin-bottom: 20px !important;
  }

  .mb-24 {
    margin-bottom: 24px !important;
  }

  .mb-32 {
    margin-bottom: 32px !important;
  }

  .mb-36 {
    margin-bottom: 36px !important;
  }

  .mb-40 {
    margin-bottom: 40px !important;
  }

  .mb-44 {
    margin-bottom: 44px !important;
  }

  .mb-48 {
    margin-bottom: 48px !important;
  }

  .mb-50 {
    margin-bottom: 50px !important;
  }

  .mb-56 {
    margin-bottom: 50px !important;
  }

  .mb-60 {
    margin-bottom: 60px !important;
  }

  .mb-64 {
    margin-bottom: 64px !important;
  }

  .mr-2 {
    margin-right: 2px !important;
  }

  .mr-4 {
    margin-right: 4px !important;
  }

  .mr-8 {
    margin-right: 8px !important;
  }

  .mr-10 {
    margin-right: 10px !important;
  }

  .mr-16 {
    margin-right: 20px !important;
  }

  .mr-20 {
    margin-right: 20px !important;
  }

  .ml-4 {
    margin-left: 8px !important;
  }

  .ml-8 {
    margin-left: 8px !important;
  }

  .ml-16 {
    margin-left: 16px !important;
  }

  .ml-18 {
    margin-left: 18px !important;
  }

  .ml-36 {
    margin-left: 36px !important;
  }

  /**
  * padding
  */

  .pt-20 {
    padding-top: 20px;
  }

  .pt-40 {
    padding-top: 40px;
  }

  .pb-20 {
    padding-bottom: 20px;
  }

  .pl-24 {
    padding-left: 24px;
  }

  /**
  * line height
  */

  .lh-1 {
    line-height: 1em !important;
  }

  .lh-1_2 {
    line-height: 1.2em !important;
  }

  /**
  * display
  */

  .d-flex {
    display: -webkit-box;
    display: flex;
  }

  .d-table {
    display: table;
  }

  .d-tcell {
    display: table-cell;
  }

  .js-sb {
    justify-content: space-between;
  }

  .js-center {
    align-items: center;
    justify-content: center;
  }

  /**
  * position
  */

  .pos-rel {
    position: relative;
  }

  .pos-none {
    position: none;
  }

  .pos-block {
    position: block;
  }

  /**
  * text-align
  */

  .ta-left {
    text-align: left;
  }

  .ta-right {
    text-align: right;
  }

  .ta-center {
    text-align: center;
  }

  /**
  * vertical-align
  */

  .va-middle {
    vertical-align: middle;
  }

  /**
  * font
  */

  .f-bold {
    font-weight: bold;
  }

  .f-light {
    font-weight: lighter;
  }

  /**
  * letter spacing
  */

  .ls-sm {
    letter-spacing: -0.1em;
  }

  .ls-md {
    letter-spacing: -0.05em;
  }

  .ls-lg {
    letter-spacing: 0.1em;
  }

</style>
<style scoped>

</style>
