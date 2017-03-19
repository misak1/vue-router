<template lang="jade">
.batch-html
  .action
    .detail-text データベースにファイル一覧データを作成します
    .toggle-button
      input#lbl-btn01(type='checkbox', name='check[]', value='1', onclick='$("#lbl-btn01").click(function( event ) {event.stopPropagation();$(this).prop("checked", true);}); App.execSiteScan();')
      label.btn.btn-primary(for='lbl-btn01') サイトスキャン
    .btn-group.btn-block.clearfix(role='group', aria-label='...')
      // button.btn.btn-default(onclick='$("#lbl-btn01").prop("checked", false);') ボタンを戻す
      button.btn.btn-default.js-cancel(onclick='App.kill();') 処理を中止する
      button.btn.btn-success(onclick='$(this).click(function( event ) {event.stopPropagation(); App.execSiteScanResume();});') 再開する
  .action
    .detail-text データベースのファイル一覧を使ってHTMLファイルをダウンロードします。
    .toggle-button
      input#lbl-btn02(type='checkbox', name='check[]', value='1', onclick='$("#lbl-btn02").click(function( event ) {event.stopPropagation();$(this).prop("checked", true);}); App.execSiteValidationEx();')
      label.btn.btn-primary(for='lbl-btn02') HTMLダウンロード
    .btn-group.btn-block.clearfix(role='group', aria-label='...')
      // button.btn.btn-default(onclick='$("#lbl-btn02").prop("checked", false);') ボタンを戻す
      button.btn.btn-default.js-cancel(onclick='App.kill();') 処理を中止する
      button.btn.btn-default(onclick='$(".header-menu .item").eq(2).find("a").click();') ダウンロードしたデータを確認する
  .action
    .detail-text ダウンロードしたHTMLをもとにPickles2用のサイトマップCSVを作成します。
    .toggle-button
      input#lbl-btn03(type='checkbox', name='check[]', value='1', onclick='$("#lbl-btn03").click(function( event ) {event.stopPropagation();$(this).prop("checked", true);}); App.execSiteValidationCsv();')
      label.btn.btn-primary(for='lbl-btn03') サイトマップCSV作成
    .btn-group.btn-block.clearfix(role='group', aria-label='...')
      // button.btn.btn-default(onclick='$("#lbl-btn03").prop("checked", false);') ボタンを戻す
      button.btn.btn-default.js-cancel(onclick='App.kill();') 処理を中止する
      button.btn.btn-default(onclick='Load.sitemapCSV();') 作成済みのCSVデータを確認する
  .action
    .detail-text 指定したCSSセレクタを元に、HTMLコードの抜き出し（スクレイピング)します。
    .toggle-button
      input#lbl-btn04(type='checkbox', name='check[]', value='1', onclick='$("#lbl-btn04").click(function( event ) {event.stopPropagation();$(this).prop("checked", true);}); App.execHtmlScraping();')
      label.btn.btn-primary(for='lbl-btn04') WEBスクレイピング
    .btn-group.btn-block.clearfix(role='group', aria-label='...')
      // button.btn.btn-default(onclick='$("#lbl-btn04").prop("checked", false);') ボタンを戻す
      button.btn.btn-default.js-cancel(onclick='App.kill();') 処理を中止する
      button.btn.btn-default(onclick='$(".header-menu .item").eq(3).find("a").click();') データを確認する
      button.btn.btn-default(onclick='App.openSiteScan();') フォルダを開く
// .btn-group(role='group', aria-label='...')
// button.btn.btn-default(type='button') Left
// button.btn.btn-default(type='button') Middle
// button.btn.btn-default(type='button') Right

</template>

<script>
import compA from '../components/a.vue'
import compB from '../components/b.vue'
export default {
  data () {
    return {
      msg: 'This is Foo!'
    }
  },
  components: {
    'comp-a': compA,
    'comp-b': compB
  },
  ready: function () {
    console.log("foo");
    this.$dispatch('_locationchange');
  }
}
</script>
