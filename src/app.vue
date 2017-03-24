<style lang="stylus">
/* reset */
html,
body,
#app {
  height: 100%;
  font-family: sans-serif;
}


/* vue style */
/*.v-link-active{
  color: red;
}*/
[v-cloak]{
  display: none;
}


/* FileZilla風レイアウト */
body {
  margin: 0px;
  background: none 0px 0px repeat scroll #efefef;
  overflow: hidden;
  position: relative;
  margin: 0px;
  padding: 0px;
  background-color: #292929 !important;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 14px;
  line-height: 1.42857;
  color: #333;
  background-color: #fff;
}
div {
  margin: 0px;
  padding: 0px;
}
#div_C {
  background-color: #ebebeb !important;
  position: relative;
}
#LeftPanel {
  width: 80%;
  float: left;
}
#RightPanel {
  width: 20%;
  float: right;
}
.handler_vertical {
  cursor: col-resize;
  width: 8px;
  float: left;
}
.handler_horizontal {
  cursor: row-resize;
  height: 8px;
  width: 100%;
  float: left;
}
.window {
  border: 1px solid #adadad;
  width: 100%;
  float: left;
  box-sizing: border-box;
  overflow: auto;
}
.top {
  height: 100%;
  position: relative;
  background-color: #ebebeb;
}
.main {
  height: 100%;
}
#content-header {
  overflow-x: auto;
  background: #fff;
  height: 80px;
  padding: 15px 0;
  box-sizing: border-box;
}
#content {
  height: 80%;
}
#content-footer {
  height: 100px;
  border: 1px solid #0f0f0f;
  padding-bottom: 50px;
}
.consolePanelMenu {
  height: 35px;
  width: 100%;
  display: table;
}
.consolePanelMenu .btn-group-sm {
  margin: 2px 2px 0px;
}
.consolePanelMenu .btn-group-sm.console-btn-group {
  margin: 10px 2px 0px 10px;
}
#consolePanel .layer-panel {
  background-color: #292929;
  padding: 4px 10px;
  box-sizing: border-box;
}
.layer-panel {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0px;
  left: 0px;
  padding: 4px;
  box-sizing: border-box;
}
.triangle-top {
  width: 0px;
  height: 0px;
  border-style: solid;
  border-width: 0px 4px 4px;
  border-color: transparent transparent #fff;
  line-height: 0px;
}
.triangle-right {
  display: inline-block;
  width: 0px;
  height: 0px;
  border-style: solid;
  border-width: 4px 0px 4px 4px;
  border-color: transparent transparent transparent #fff;
  line-height: 0;
}
.triangle-left {
  display: inline-block;
  width: 0px;
  height: 0px;
  border-style: solid;
  border-width: 4px 4px 4px 0px;
  border-color: transparent #fff transparent transparent;
  line-height: 0;
}
.hideRight #LeftPanel {
  width: 100% !important;
}
.hideLeft #RightPanel {
  width: 100% !important;
}
#btnShowFooter {
  position: absolute;
  bottom: 0px;
  left: 50%;
  display: none;
  width: 52px;
  height: 23px;
  background: #333;
  border-radius: 3px 3px 0px 0px;
  border-width: 1px 1px 0px;
  border-top-style: solid;
  border-right-style: solid;
  border-left-style: solid;
  border-top-color: #fff;
  border-right-color: #fff;
  border-left-color: #fff;
  border-image: initial;
  border-bottom-style: initial;
  border-bottom-color: initial;
  margin-left: -25px;
  text-align: center;
  box-sizing: border-box;
}
#btnShowFooter a {
  color: #fff;
  display: block;
  margin-top: -8px;
  cursor: pointer;
}
#btnShowLeft {
  position: absolute;
  top: 50%;
  left: 0px;
  display: none;
  width: 23px;
  height: 52px;
  background: #333;
  border-radius: 0px 3px 3px 0px;
  border-width: 1px 1px 1px 0px;
  border-top-style: solid;
  border-right-style: solid;
  border-bottom-style: solid;
  border-top-color: #fff;
  border-right-color: #fff;
  border-bottom-color: #fff;
  border-image: initial;
  border-left-style: initial;
  border-left-color: initial;
  text-align: center;
  box-sizing: border-box;
}
#btnShowLeft a {
  color: #fff;
  display: block;
  cursor: pointer;
  height: 100%;
}
#btnShowRight {
  position: absolute;
  top: 50%;
  right: 0px;
  display: none;
  width: 23px;
  height: 52px;
  background: #333;
  border-radius: 3px 0px 0px 3px;
  border-width: 1px 0px 1px 1px;
  border-top-style: solid;
  border-bottom-style: solid;
  border-left-style: solid;
  border-top-color: #fff;
  border-bottom-color: #fff;
  border-left-color: #fff;
  border-image: initial;
  border-right-style: initial;
  border-right-color: initial;
  text-align: center;
  box-sizing: border-box;
}
#btnShowRight a {
  color: #fff;
  display: block;
  cursor: pointer;
  height: 100%;
}
#btnShowLeft .triangle-right,
#btnShowRight .triangle-left {
  margin-top: 19px;
}
.textareamodal {
  position: fixed;
  z-index: 1060;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.702);
  top: 0px;
  left: 0px;
  display: none;
}
.textareamodal-dialog {
  background: #fff;
  position: relative;
  top: 50%;
  left: 50%;
  height: 482px;
  margin-top: -241px;
  width: 600px;
  margin-left: -300px;
  text-align: center;
  padding: 37px 30px;
}
.textareamodal-dialog-textarea {
  width: 100%;
  height: 310px;
  resize: none;
  line-height: 1.2;
  font-size: 12px;
  padding: 4px;
}
.textareamodal-dialog-close {
  position: absolute;
  top: 20px;
  right: 20px;
}
.textareamodal-dialog-close a {
  color: #148fcc;
}
.textareamodal-dialog-title {
  font-size: 24px;
  font-weight: bold;
  margin: 0px 0px 18px;
}

/* navi */
#navigation {
  position: relative;
  /*background-color: #fff;
  box-shadow: 0 0 12px rgba(0, 0, 0, 0.26);*/
}
#navigation ul li {
  display: inline-block;
}
#navigation ul li a {
  display: inline-block;
  margin:0;
  font-size: 16px;
  text-decoration: none;
}
#navigation ul li.current-item a {
  color: #999999;
}
#navigation #slide-line {
  position: absolute;
  bottom: 0;
  height: 2px;
  background-color: #000;
  -webkit-transition: all .3s ease;
  transition: all .3s ease;
}
/* /navi */

/* footer */
#content-footer{
  .consolePanelMenu{
    color:#fff;
    a{
      cursor:pointer;
      &:hover{
        filter: brightness(1.1);
      }
    }
  }
  .consolePanelMenu {
      height: 35px;
      width: 100%;
      display: table;
      .btn-group-sm.console-btn-group {
          margin: 10px 2px 0 10px;
      }
  }
  #consolePanel {
      width: 100%;
      height: 100%;
      padding-bottom: 50px;
      textarea,
      .div-textarea{
        height: 100%;
        font-family: Osaka-mono, "MS Gothic", monospace;
        padding: 0 8px;
        background-color: #0f0f0f;
        color: #b2b2b2;
        -webkit-font-smoothing: antialiased;
        letter-spacing: .1em;
        line-height: 1em;
      }
      .div-textarea div {
          white-space: pre-wrap;
      }
  }
  .console-btn-group a{
    margin-left:15px;
    &:first-child{
      margin-left:0;
    }
  }
  .layer-wrap {
    position: relative;
    width: 100%;
    height: 100%;
  }
  .layer-panel.is-current {
    display: block;
  }
}

</style>

<template lang="jade">
p(v-show="loading" style="color:red") loading...
.main
  #content-header
    ul.header-menu.nav.nav-tabs
      // 一番最初に表示したいページに.is-current

      nav#navigation
        ul
          li.current-item
            a(v-link='/') 通常設定
          li
            a(v-link='/foo') 処理／実行
          li
            a(v-link='/bar/1') 開発
          li
            a(v-link='/ggg') サポート
        |   
        span#slide-line
  #content(style='')
    #LeftPanel.Panel(style='')
      #div_A.window.top
        router-view.view(v-transition='test', transition-mode='out-in')
        #btnShowRight
          a
            span.triangle-left
      #div_left.handler_horizontal
    #div_vertical.handler_vertical
    #RightPanel.Panel(style='')
      #div_C.window.top
        #rightContent
        #btnShowLeft
          a
            span.triangle-right
      #div_right.handler_horizontal
    #btnShowFooter
      a
        span.triangle-top
  #content-footer(style='')
    .consolePanelMenu
        .btn-group-sm.console-btn-group(role='group', aria-label='...')
            a.u-mr10(onclick="Console.clear();") バッファクリア
            a.u-mr10(onclick="App.toggleDevTools();") Developer Tools
    #consolePanel
      .layer-wrap
        .layer-panel
          // 設定
          .m-console.div-textarea
            - var n = 100
            while n > 0
              div
              - n--

</template>


<script>
export default {
  data() {
    return {
      loading: false
    }
  }
  ,
  created() {
    this.$on('_locationchange', () => {
      //console.log('_locationchange');
      //console.log(location.pathname);

      var comp1 = location.pathname.split('/');
      if (comp1.length >= 2) {
        var idx = 0;
        $.each($('#navigation a'), function (i, v) {
          var comp2 = v.getAttribute('href').split('/');
          if (comp2.length >= 2 && comp1[1] == comp2[1]) {
            idx = i;
          }
        });
        $('#navigation li').removeClass('current-item').eq(idx).addClass('current-item');
      }
    });
  }
  ,
  ready: function () {
    /**
    * FileZilla風レイアウト
    */
    $(function () {
      window.onresize = resize;
      //window.onload = resize;
      resize();
      //console.log('resize');
      $.resizable('div_vertical', "v");
      $.resizable('div_right', "h");
      $.resizable('div_left', "h");
    });

    var $content = $("#content");
    var headerHeight = $('#content-header').height();
    var content_margin_side = 30;
    var footer_margin_bottom = 5;
    var border_width_x4 = (parseInt($('.window.top').css('border-left-width')) * 2) + (parseInt($('.window.top').css('border-right-width')) * 2)
    var divHeight = $("#div_left").height();
    var winHeight;

    var floatFormat = function (number, n) {
      var _pow = Math.pow(10, n);

      return Math.ceil(number * _pow) / _pow;
    }

    var resize = function (isVertical) {
      var _verticalResize = isVertical || false;
      if (typeof _verticalResize !== 'boolean') {
        _verticalResize = false;
      }

      if ($content.hasClass('is-Single')) {
        // //console.log('not resize');
        return true;
      }
      winHeight = (window.innerHeight || (window.document.documentElement.clientHeight || window.document.body.clientHeight));

      var ratio = floatFormat($content.height() / winHeight, 2);
      //var panelHeight = Math.ceil((winHeight - divHeight) * ratio);
      var panelHeight = Math.round((winHeight - divHeight) * ratio);

      $("#content").css({
        "min-height": panelHeight
      });
      $("#div_vertical").css({
        "height": panelHeight
      });
      $("#LeftPanel").css({
        "height": panelHeight - divHeight
      });

      // var content_width = $("#content").width();
      var content_width = $("body").width(); // DebToolの表示時に正しい値が取れない為
      var RightPanelWidth = content_width - $("#LeftPanel").width() - $("#div_vertical").width() - border_width_x4;
      if (_verticalResize) {
        $("#RightPanel").css({
          "height": panelHeight - divHeight,
        });
      } else {
        $("#RightPanel").css({
          "height": panelHeight - divHeight,
          "width": RightPanelWidth
        });
        // 念のため
        var LeftPanelWidth = content_width - $("#RightPanel").width() - $("#div_vertical").width() - border_width_x4;
        $("#LeftPanel").css({
          "width": LeftPanelWidth
        });
      }
      $("#content-footer").height(winHeight - (headerHeight + panelHeight + footer_margin_bottom));
    }
    $('#btnShowFooter a').on('click', function () {
      footerShow(true);
      setTimeout(function () {
        // skipW = true;
        // window.resize();
        resize(true);
      }, 300);
    });
    $('#btnShowRight a').on('click', function () {
      leftPanelShow(true);
      setTimeout(function () {
        resize();
      }, 300);
    });
    $('#btnShowLeft a').on('click', function () {
      rightPanelShow(true);
      setTimeout(function () {
        resize();
      }, 300);
    });
    var leftPanelShow = function (isShow) {
      setTimeout(function (isShow) {
        if (!isShow) {
          $("#div_vertical, #RightPanel").hide();
          $("#LeftPanel").css({ width: '100%' });
          $('#btnShowRight').css({ display: 'inline-block' });
          $('html').addClass('hideRight');
        } else {
          $("#LeftPanel").css({ width: '80%' });
          $("#RightPanel").css({ width: '20%' });
          $("#div_vertical, #RightPanel").show();
          $('#btnShowRight').hide();
          $('html').removeClass('hideRight');
        }
      }, 300, isShow);
    }
    var rightPanelShow = function (isShow) {
      setTimeout(function (isShow) {
        if (!isShow) {
          $("#div_vertical, #LeftPanel").hide();
          $("#RightPanel").css({ width: '100%' });
          $('#btnShowLeft').css({ display: 'inline-block' });
          $('html').addClass('hideLeft');
        } else {
          $("#RightPanel").css({ width: '80%' });
          $("#LeftPanel").css({ width: '20%' });
          $("#div_vertical, #LeftPanel").show();
          $('#btnShowLeft').hide();
          $('html').removeClass('hideLeft');
        }
      }, 300, isShow);
    }

    var footerShow = function (isShow) {
      setTimeout(function (isShow) {
        if (!isShow) {
          $("#content-footer").hide();
          $("#content").css({ minHeight: '', height: '100%' });
          $("#LeftPanel, #RightPanel").css({ height: '100%' });
          $('#btnShowFooter').css({ display: 'inline-block' });
          $('html').addClass('hideFooter');
        } else {
          $("#content-footer").show();
          $("#content").css({ minHeight: '80%', height: '80%' });
          $("#LeftPanel, #RightPanel").css({ height: '80%' });
          $('#btnShowFooter').hide();
          $('html').removeClass('hideFooter');
        }
      }, 300, isShow);
    }

    $.resizable = function (resizerID, vOrH) {
      //console.log("resizable");
      $('#' + resizerID).bind("mousedown", function (e) {
        var start = vOrH === 'v' ? e.pageX : e.pageY;
        var height = $content.height();
        var leftwidth = $('#' + resizerID).prev().width();
        var rightwidth = $('#' + resizerID).next().width();


        var mouseMove = function (e) {
          var end = vOrH === 'v' ? e.pageX : e.pageY;
          if (vOrH == 'h') {
            // タテ
            var newHeight = height + (end - start);
            if (newHeight > content_margin_side || newHeight < 0) {
              $content.height(newHeight);

              $("#content").css({
                "min-height": newHeight
              });
              $("#div_vertical").css({
                "height": newHeight
              });
              $("#LeftPanel, #RightPanel").css({
                "height": newHeight - divHeight
              });
              $("#content-footer").height(winHeight - (headerHeight + newHeight + footer_margin_bottom));

            }
          } else {
            // ヨコ
            var newLeftWidth = leftwidth + (end - start);
            var newRightWidth = rightwidth - (end - start);

            // //console.log(newRightWidth);
            // 段落ち対策
            if (content_margin_side < newLeftWidth && newRightWidth > content_margin_side) {
              $('#' + resizerID).prev().width(newLeftWidth);
              $('#' + resizerID).next().width(newRightWidth);
            } else {
              // //console.log("holizontal-over");
            }
          }
        };
        document.addEventListener('mouseup', function (e) {
          // var start = vOrH === 'v' ? e.pageX : e.pageY;
          // var height = $content.height();
          // var leftwidth = $('#' + resizerID).prev().width();
          // var rightwidth = $('#' + resizerID).next().width();
          // var end = vOrH === 'v' ? e.pageX : e.pageY;
          // //console.log('mouseup', e.pageX , e.pageY)

          if ($content.height() > $(window).height() - $('#content-header').height() - 40) {
            // //console.log("vertical-over");
            e.preventDefault(); // drag キャンセル
            footerShow(false);
          }
          var newRightWidth = $('#div_right').prev().width();
          var newLeftWidth = $('#div_left').prev().width()

          e.preventDefault(); // drag キャンセル
          // //console.log('newLeftWidth',newLeftWidth,"newRightWidth", newRightWidth, "content_margin_side", content_margin_side);
          if (newRightWidth <= (content_margin_side + 20)) {
            leftPanelShow(false);
          } else if (newLeftWidth <= (content_margin_side + 20)) {
            rightPanelShow(false);
          }
          // //console.log("holizontal-over");


          document.removeEventListener("mousemove", mouseMove);
          document.removeEventListener("mouseup", this);
        });
        document.addEventListener('mousemove', mouseMove);
      });
    }

    /**
    * navigation
    */
    $(function () {
      var $nav = $("#navigation"),
        $slideLine = $("#slide-line"),
        $currentItem = $(".current-item");

      $(function () {
        // Menu has active item
        if ($currentItem[0]) {
          var _$this = $nav.find('li.current-item');
          $slideLine.css({
            "width": _$this.width(),
            "left": _$this.position().left + parseInt(_$this.css('marginLeft'))
          });
        }

        // Underline transition
        $($nav).find("li").hover(
          // Hover on
          function () {
            $slideLine.css({
              "width": $(this).width(),
              "left": $(this).position().left + parseInt($(this).css('marginLeft'))
            });
          },
          // Hover out
          function () {
            if ($currentItem[0]) {
              // Go back to current
              var _$this = $nav.find('li.current-item');
              $slideLine.css({
                "width": _$this.width(),
                "left": _$this.position().left + parseInt(_$this.css('marginLeft'))
              });
            } else {
              // Disapear
              $slideLine.width(0);
            }
          }
        );
      });

      // 横並び間隔揃え
      var max_w = 0;
      $.when(
        $.each($('#navigation li'), function () {
          var w = $(this).width();
          max_w = (max_w < $(this).width()) ? w : max_w;
        })
      )
        .done(function () {
          // 最大幅
          // //console.log(max_w);
          var new_w = max_w + 20;
          $.each($('#navigation li'), function () {
            var side = new_w - $(this).width() / 2;
            $(this).css({ marginLeft: side + 'px', marginRight: side + 'px' });
          })
          //   margin-right: 45px;
        });

      if ("onhashchange" in window) {
        console.log("お使いのブラウザは hashchange イベントをサポートしています");
      }

      function locationHashChanged() {
        //console.log(location.url);
      }

      window.onhashchange = locationHashChanged;
    });
  }
}
</script>
