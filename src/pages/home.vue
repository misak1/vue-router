<template lang="jade">
.setting
  h1 {{title}}
  fieldset
    legend 環境設定
    .field_group
      // p
      // label.col-sm-12.control-label PHPパス
      // .col-sm-12.uploadButton
      // span(style="width: 15%;display: inline-block; vertical-align: top;") ファイルを選択
      // input(type="file" id="uv1_file" onchange="uv1.style.display='inline-block'; uv1.value = this.value;" required)
      // input(type="text" id="uv1" name='PHP_PATH' class="uploadValue" disabled)
      p
        label.col-sm-12.control-label Asazukeパス
        .col-sm-12.uploadButton
          span(style='width: 15%;display: inline-block; vertical-align: top;') ディレクトリを選択
          input#uv2_file(type='file', onchange="uv2.style.display='inline-block'; uv2.value = this.value;", webkitdirectory='webkitdirectory', directory='directory', required='required')
          input#uv2.uploadValue(type='text', name='ASAZUKE_DIR_PATH', disabled='disabled')
      .col-sm-12.u-mt10
        input.btn.btn-default(type='button', value='パス変更', onclick='Setting.paths();')
        input.btn.btn-default(type='button', value='Asazukeのインストール', onclick='App.asazuke_install();')
        input.btn.btn-default.js-asazuke-update(type='button', value='Asazukeのアップデート', onclick='App.asazuke_update();')
  fieldset.u-mt10
    legend プロジェクト設定
    .field_group
      h5 プロジェクトを作成
      p.new_project
        input.btn.btn-default(type='button', value='新規プロジェクト', onclick='Setting.addProject();')
      h5 既存のプロジェクトから選択
      .form-group
        label.col-sm-2.control-label プロジェクトを選択して下さい。
        .col-sm-10
          select.form-control.js-projectList.project_lists(onchange='Setting.selectProject($(this).val());')
  fieldset.setting_target.u-mt10
    legend 解析対象サイト
    .field_group
      p
        label
          | サイトURL：
          input(type='text', name='SITE_URL', size='40', value='', placeholder='http://www.sample.jp')
      p
        label
          | ディレクトリ：
          input(type='text', name='START_PATH', size='40', value='', placeholder='/')
      p
        label
          | ユーザ：
          input(type='text', name='AUTH_USER', size='40', value='', placeholder='auth_user')
      p
        label
          | パスワード：
          input(type='text', name='AUTH_PASS', size='40', value='', placeholder='auth_password')
      .col-sm-12
        input.btn.btn-default(type='button', value='確定', onclick='Setting.target();')
  // p
  // input#setting_modify_all(type='button', value='すべて確定' onclick="Setting.all();")

</template>

<script>
export default {
  data () {
    return {
      title: '通常設定'
    }
  }
  ,
  ready: function () {
    console.log("home");
    this.$dispatch('_locationchange');
    $('#rightContent').html('<p>test<p>');
  }
  // components: {
  //   'comp-a': compA,
  //   'comp-b': compB
  // },
}
</script>

<style lang="stylus">
font-stack = Helvetica, sans-serif
primary-color = #999
body
  font 100% font-stack
  color primary-color
</style>
