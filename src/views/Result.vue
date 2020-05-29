<template>
  <div class="flex-col" id="app">
    <div class="el-dialog__wrapper" style="display: none;" data-v-0a80d877>
      <div class="el-dialog el-dialog--center login-dialog" style="width: 360px; margin-top: 15vh;">
        <div class="el-dialog__header">
          <span class="el-dialog__title"></span>
          <button class="el-dialog__headerbtn" aria-label="Close" type="button">
            <i class="el-dialog__close el-icon el-icon-close"></i>
          </button>
        </div>
        <!---->
        <!---->
      </div>
    </div>
    <div data-v-6ac91252>
      <div class="el-dialog__wrapper collect-dialog" style="display: none;" data-v-6ac91252>
        <div class="el-dialog el-dialog--center" style="width: 500px; margin-top: 15vh;">
          <div class="el-dialog__header">
            <span class="el-dialog__title"></span>
            <button class="el-dialog__headerbtn" aria-label="Close" type="button">
              <i class="el-dialog__close el-icon el-icon-close"></i>
            </button>
          </div>
          <!---->
          <!---->
        </div>
      </div>
    </div>
    <div class="el-dialog__wrapper feedback-dialog" style="display: none;" data-v-7018e13e>
      <div class="el-dialog el-dialog--center" style="width: 500px; margin-top: 15vh;">
        <div class="el-dialog__header">
          <span class="el-dialog__title">反馈建议</span>
          <button class="el-dialog__headerbtn" aria-label="Close" type="button">
            <i class="el-dialog__close el-icon el-icon-close"></i>
          </button>
        </div>
        <!---->
        <!---->
      </div>
    </div>
    <div class="flex-col" data-v-130acafa>
      <div class="flex-row headerbar" data-v-130acafa>
        <div class="flex-row main-align-space-between cross-align-end inner" data-v-130acafa>
          <div class="flex-row cross-align-end" data-v-130acafa>
            <a class="logo flex-row cross-align-center router-link-active" href="/" data-v-130acafa></a>
            <div class="flex-col" data-v-130acafa>
              <div data-v-130acafa data-v-73d3fb0a>
                <div class="search-box" data-v-73d3fb0a>
                  <div class="el-input el-input-group el-input-group--append" data-v-73d3fb0a>
                    <input
                      class="el-input__inner"
                      type="text"
                      maxlength="1000"
                      placeholder="请输入案情描述、关键词、案由、案号..."
                      data-v-73d3fb0a
                      v-model="input"
                    />
                    <div class="el-input-group__append" data-v-73d3fb0a @click="doSearch">
                      <i class="el-icon-search" data-v-73d3fb0a></i>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="flex-col main">
      <div class="detail-wrapper inner" data-v-2da6a776>
        <div class="flex-row" data-v-2da6a776>
          <div class="flex-col flex-1 wenshu box-shadow" data-v-2da6a776>
            <div class="flex-col" data-v-2da6a776>
              <div class="wenshu-header" data-v-2da6a776>
                <!---->
                <span class="wenshu-title" data-v-2da6a776>
                  {{this.ah}}
                </span>
                <div class="flex-row sep-wrapper wenshu-info" data-v-2da6a776 data-v-6856ea31>
                  <span class="sep-item" data-v-6856ea31>{{this.jbfy}}</span>
                  <span class="sep-item sep-offset-left" data-v-6856ea31>{{this.ah}}</span>
                  <span class="sep-item" data-v-6856ea31>{{this.lkrq}}</span>
                </div>
              </div>
              <div class="flex-col wenshu-content" data-v-2da6a776>
                <div data-v-2da6a776>
                  <h2 id="SBDSR" data-v-2da6a776>当事人信息</h2>
                  <div class="text_wrap">
                    {{this.dsr}}
                    <p></p>
                  </div>
                </div>
                <div data-v-2da6a776>
                  <h2 id="SSJL" data-v-2da6a776>诉讼记录</h2>
                  <div class="text_wrap">
                    {{this.ssjl}}
                    <p></p>
                  </div>
                </div>
                <div data-v-2da6a776>
                  <h2 id="SS" data-v-2da6a776>案件基本情况</h2>
                  <div class="text_wrap">
                    {{this.ajjbqk}}
                    <p></p>
                  </div>
                </div>
                <div data-v-2da6a776>
                  <h2 id="LY" data-v-2da6a776>裁判分析过程</h2>
                  <div class="text_wrap">
                    {{this.cpfxgc}}
                    <p></p>
                  </div>
                </div>
                <div data-v-2da6a776>
                  <h2 id="JG" data-v-2da6a776>裁判结果</h2>
                  <div class="text_wrap">
                    {{this.pjjg}}
                    <p></p>
                  </div>
                </div>
                <div data-v-2da6a776>
                  <h2 id="WB" data-v-2da6a776>文尾</h2>
                  <div class="text_wrap">
                    {{this.ww}}
                    <p></p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "Home",
  data() {
    return {
      input: "",
      get_text: "",
      title: "",
      jbfy: "",
      content: "",
      lkrq: "",
      ah: "",
      dsr:"",
      ssjl: "",
      ajjbqk: "",
      cpfxgc: "",
      pjjg: "",
      ww: ""
    };
  },
  mounted: function() {
    console.log(
      "get " + this.$route.query.item
    );
    this.input = "";
    this.get_text = "http://127.0.0.1:8010/detail/common/?rnum=" + this.$route.query.item;
    axios
      .get(
        this.get_text
      )
      .then(response => {
        this.itemData = new Array();
        console.log(response.data);
        this.ah = response.data.AH;
        this.dsr = response.data.DSR;
        this.ssjl = response.data.SSJL;
        this.ajjbqk = response.data.AJJBQK;
        this.cpfxgc = response.data.CPFXGC;
        this.pjjg = response.data.PJJG;
        this.ww = response.data.WW;
        this.jbfy = response.data.JBFY;
        this.lkrq = response.data.LKRQ;
      })
      .catch(error => console.log(error));
  },
  methods: {
    doSearch(e) {
      console.log("click " + this.input, e);
      this.$router.push({
        path: "/search",
        query: { key: this.input, page: 1 }
      });
    }
  }
};
</script>

<style>
* {
  outline: none;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
.flex-col {
  -webkit-box-orient: vertical;
  -ms-flex-direction: column;
  flex-direction: column;
}
a {
  text-decoration: none;
  color: inherit;
}
.flex-col,
.flex-row {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-direction: normal;
}
#app {
  min-height: 100%;
}
body {
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto,
    Helvetica Neue, Helvetica, PingFang SC, Hiragino Sans GB, Microsoft YaHei,
    SimSun, sans-serif;
  -webkit-font-smoothing: antialiased;
  line-height: 1.5;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  overflow: auto;
}
html {
  font-size: 37.5px;
}
body,
html {
  height: 100%;
}
body {
  background-color: #f9fbfb;
  min-width: 1200px;
  min-height: 512px;
  word-break: break-all;
  word-wrap: break-word;
  color: #666;
  font-size: 14px;
}
.el-dialog__wrapper {
  position: fixed;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
  overflow: auto;
  margin: 0;
}
.main {
  -webkit-box-flex: 1;
  -ms-flex-positive: 1;
  flex-grow: 1;
  min-height: 500px;
}
.flex-row {
  -webkit-box-orient: horizontal;
  -ms-flex-direction: row;
  flex-direction: row;
}
.main-align-center {
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
}
.cross-align-center {
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}
[data-v-0b81b07c].footer {
  -ms-flex-negative: 0;
  flex-shrink: 0;
  background: #fafbfd;
  color: #666;
  line-height: 2em;
  font-size: 12px;
  text-align: center;
  padding: 20px 0;
  border-top: 1px solid #eaedf3;
}
[data-v-2e0417d0].back-top {
  -webkit-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
  position: fixed;
  z-index: 1000;
  bottom: 120px;
  right: 20px;
}
.back-top [data-v-2e0417d0].backtop-item-arrow {
  display: none;
}
.item-wrapper + [data-v-2e0417d0].item-wrapper {
  margin-top: 6px;
}
[data-v-2e0417d0].item {
  width: 45px;
  height: 45px;
  color: #c3d0ea;
  font-size: 25px;
  cursor: pointer;
  background-color: #fff;
  -webkit-box-shadow: 0 2px 4px 0 hsla(0, 0%, 85.1%, 0.5);
  box-shadow: 0px 2px 4px 0px hsla(0, 0%, 85%, 0.5);
  padding: 10px;
  border-radius: 4px;
}
i {
  font-style: normal;
}
[class*=" el-icon-"],
[class^="el-icon-"] {
  font-family: element-icons !important;
  speak: none;
  font-style: normal;
  font-weight: 400;
  font-variant: normal;
  text-transform: none;
  line-height: 1;
  vertical-align: baseline;
  display: inline-block;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.toolbar .toolbar-item i[data-v-2da6a776] {
  font-size: 27px;
  line-height: 1;
}
#app [class*=" el-icon-my"],
#app [class^="el-icon-my"] {
  font-family: iconfont !important;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.el-popover {
  position: absolute;
  background: #fff;
  min-width: 150px;
  border-radius: 4px;
  border: 1px solid #ebeef5;
  padding: 12px;
  z-index: 2000;
  color: #666;
  line-height: 1.4;
  text-align: justify;
  font-size: 14px;
  -webkit-box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);
  box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.1);
}
.backtop-popover.el-popover {
  padding: 0 !important;
}
[data-v-2e0417d0].backtop-popover-inner {
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}
img[data-v-2e0417d0] {
  width: 160px;
  height: 160px;
  margin-top: 10px;
  margin-bottom: 5px;
}
img[data-v-2e0417d0].qrcode {
  width: 165px;
  height: 165px;
  margin-top: 5px;
  margin-bottom: 0px;
}
p[data-v-2e0417d0] {
  color: #333;
  font-size: 12px;
  line-height: 1.5;
}
p[data-v-2e0417d0]:last-child {
  margin-bottom: 10px;
}
[data-v-0b81b07c].item {
  margin-right: 20px;
}
[data-v-0b81b07c].police-icon {
  margin-left: 1em;
  height: 16px;
  width: auto;
  margin-right: 2px;
}
[data-v-0b81b07c].line {
  width: 2px;
  height: 14px;
  background-color: #ccc;
  position: relative;
  left: -9px;
  top: 5px;
}
.cross-align-end {
  -webkit-box-align: end;
  -ms-flex-align: end;
  align-items: flex-end;
}
.inner {
  width: 1200px;
  margin: 0 auto;
}
[data-v-2da6a776].detail-wrapper {
  margin-top: 16px;
  margin-bottom: 30px;
}
.flex-1 {
  -webkit-box-flex: 1;
  -ms-flex: 1;
  flex: 1;
}
.box-shadow {
  background: #fff;
  -webkit-box-shadow: 2px 2px 8px 0 rgba(0, 0, 0, 0.08);
  box-shadow: 2px 2px 8px 0px rgba(0, 0, 0, 0.08);
}
[data-v-2da6a776].toolbar {
  width: 70px;
  -ms-flex-item-align: start;
  align-self: flex-start;
  position: fixed;
}
[data-v-2da6a776].wenshu {
  background-color: #fff;
  margin-left: 95px;
  color: #333;
}
[data-v-2da6a776].wenshu-header {
  border-bottom: 1px solid #eaedf3;
  padding: 18px 40px 23px;
}
[data-v-2da6a776].wenshu-content {
  font-size: 16px;
  color: #333;
  line-height: 28px;
  padding: 18px 40px 50px;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: 400;
}
.wenshu-content h1[data-v-2da6a776],
.wenshu-content h2[data-v-2da6a776] {
  color: #333;
  font-size: 20px;
  margin-bottom: 9px;
  line-height: 28px;
  font-weight: 500;
}
.wenshu-content p[data-v-2da6a776] {
  margin-bottom: 20px;
  text-indent: 2em;
}
em {
  color: #c00;
  font-style: normal;
}
#app .wenshu-content a[href] {
  color: #637cbc;
  cursor: pointer;
}
[data-v-2da6a776].wenshu-title {
  font-size: 28px;
  line-height: 42px;
  color: #333;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  font-weight: 500;
}
[data-v-2da6a776].wenshu-info {
  margin-top: 10px;
}
[data-v-6856ea31].sep-offset-left {
  margin-left: -0.5em;
}
.toolbar [data-v-2da6a776].toolbar-item {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  cursor: pointer;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  height: 83px;
  border-bottom: 1px solid #eaedf3;
}
.toolbar [data-v-2da6a776]:last-child.toolbar-item {
  border: none;
}
.toolbar .toolbar-item span[data-v-2da6a776] {
  margin-top: 10px;
  font-size: 12px;
  line-height: 1;
  color: #8b94aa;
}
.lishen-popper.el-popper {
  padding: 0;
}
[data-v-5ab240b0].steps-wrapper {
  padding: 20px 30px !important;
  width: 300px;
  max-height: 380px;
  overflow-y: auto;
}
[data-v-5ab240b0].step {
  height: 71px;
}
[data-v-5ab240b0]:last-child.step {
  height: auto;
}
[data-v-5ab240b0].step-head {
  -webkit-box-flex: 0;
  -ms-flex-positive: 0;
  flex-grow: 0;
  position: relative;
  width: 14px;
  color: #637cbc;
  border-color: #637cbc;
}
[data-v-5ab240b0].step-main {
  padding-left: 10px;
  -webkit-box-flex: 1;
  -ms-flex-positive: 1;
  flex-grow: 1;
}
[data-v-5ab240b0].step-title {
  display: block;
  line-height: 1;
  font-size: 14px;
  margin-bottom: 3px;
  color: #333;
}
:not(.is-disabled).step [data-v-5ab240b0].step-title {
  color: #333;
  cursor: pointer;
}
[data-v-5ab240b0].step-desc {
  font-size: 12px;
  color: #666;
  line-height: 17px;
  margin-left: -0.5em;
}
[data-v-5ab240b0].step-time {
  margin-left: 8px;
}
[data-v-5ab240b0].step-line {
  width: 1px;
  top: 3px;
  bottom: -3px;
  left: 7px;
  position: absolute;
  border-color: inherit;
  background-color: #d1d5e4;
}
[data-v-5ab240b0].step-line-inner {
  display: block;
  border-width: 1px;
  border-color: inherit;
  width: 0px;
  height: 0px;
}
[data-v-5ab240b0].step-icon,
[data-v-5ab240b0].step-line-inner {
  -webkit-transition: 0.15s ease-out;
  transition: 0.15s ease-out;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
}
[data-v-5ab240b0].step-icon {
  border-radius: 50%;
  border: 1px solid;
  border-color: inherit;
  position: absolute;
  z-index: 1;
  display: -webkit-inline-box;
  display: -ms-inline-flexbox;
  display: inline-flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  width: 14px;
  height: 14px;
  font-size: 14px;
  background: #fff;
}
[data-v-5ab240b0].step-icon-inner {
  display: inline-block;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  text-align: center;
  font-weight: 700;
  line-height: 1;
  color: inherit;
}
.step.is-current [data-v-5ab240b0].step-icon-inner {
  background-color: #637cbc;
  width: 8px;
  height: 8px;
  border-radius: 50%;
}
.step.is-disabled [data-v-5ab240b0].step-title {
  cursor: auto;
  color: #8b94aa;
}
.step.is-disabled [data-v-5ab240b0].step-desc {
  color: #c7c7c7;
}
[data-v-6bb33a9a].steps-wrapper {
  padding: 20px 27px;
  width: 250px;
}
[data-v-6bb33a9a].step {
  height: 44px;
}
[data-v-6bb33a9a]:last-child.step {
  height: auto;
}
[data-v-6bb33a9a].step-head {
  -webkit-box-flex: 0;
  -ms-flex-positive: 0;
  flex-grow: 0;
  position: relative;
  width: 14px;
  color: #637cbc;
  border-color: #637cbc;
}
[data-v-6bb33a9a].step-main {
  padding-left: 10px;
  -webkit-box-flex: 1;
  -ms-flex-positive: 1;
  flex-grow: 1;
}
[data-v-6bb33a9a].step-title {
  display: block;
  line-height: 1.4;
  margin-top: -0.2em;
  max-height: 39.2px;
  font-size: 14px;
  margin-bottom: 3px;
  color: #333;
}
:not(.is-disabled).step [data-v-6bb33a9a].step-title {
  color: #333;
  cursor: pointer;
}
[data-v-6bb33a9a].step-line {
  width: 1px;
  top: 3px;
  bottom: -3px;
  left: 7px;
  position: absolute;
  border-color: inherit;
  background-color: #d1d5e4;
}
:last-child.step [data-v-6bb33a9a].step-line {
  display: none;
}
[data-v-6bb33a9a].step-line-inner {
  display: block;
  border-width: 1px;
  border-color: inherit;
  width: 0px;
  height: 0px;
}
[data-v-6bb33a9a].step-icon,
[data-v-6bb33a9a].step-line-inner {
  -webkit-transition: 0.15s ease-out;
  transition: 0.15s ease-out;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
}
[data-v-6bb33a9a].step-icon {
  border-radius: 50%;
  border: 1px solid;
  border-color: inherit;
  position: absolute;
  z-index: 1;
  display: -webkit-inline-box;
  display: -ms-inline-flexbox;
  display: inline-flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  width: 14px;
  height: 14px;
  font-size: 14px;
  background: #fff;
}
[data-v-6bb33a9a].step-icon-inner {
  display: inline-block;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  text-align: center;
  font-weight: 700;
  line-height: 1;
  color: inherit;
}
[data-v-130acafa].headerbar {
  padding-bottom: 13px;
  -ms-flex-negative: 0;
  flex-shrink: 0;
  background-color: #fff;
  border-bottom: 1px solid #eaedf3;
  min-height: 50px;
}
.main-align-space-between {
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}
[data-v-130acafa].headerbar-right {
  position: relative;
  top: -2px;
}
[data-v-130acafa].avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  margin-right: 10px;
}
[data-v-130acafa].menu-item {
  height: 40px;
  line-height: 40px;
  font-size: 14px;
  color: #333;
  cursor: pointer;
}
[data-v-130acafa].logo {
  width: 134px;
  height: 60px;
  background-image: url("data:image/png;base64,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");
  background-position: 50%;
  background-repeat: no-repeat;
  background-size: 100% auto;
  position: relative;
  left: -5px;
  top: 7px;
}
[data-v-431171e6].category-list {
  height: 40px;
  font-size: 14px;
  color: #666;
  position: relative;
  top: 3px;
}
[data-v-73d3fb0a].search-box {
  position: relative;
}
[data-v-73d3fb0a].suggestion {
  max-width: 536px;
  width: 536px;
  background-color: #fff;
  border-top: 0;
  z-index: 1002;
  color: #333;
  font-size: 14px;
  position: absolute;
}
.one-line,
.two-line {
  overflow: hidden;
  text-overflow: ellipsis;
}
[data-v-73d3fb0a].suggestion-item {
  height: 32px;
  overflow: hidden;
  line-height: 26px;
  padding: 3px 15px;
  cursor: pointer;
}
[data-v-73d3fb0a].suggestion-header {
  background: #f4f7f9;
  color: #849aae;
  cursor: auto;
}
.one-line {
  white-space: nowrap;
  display: block;
}
[data-v-73d3fb0a].clear-history {
  cursor: pointer;
}
.el-input {
  position: relative;
  font-size: 14px;
  display: inline-block;
  width: 100%;
}
.el-input-group {
  line-height: normal;
  display: inline-table;
  width: 100%;
  border-collapse: separate;
  border-spacing: 0px;
}
[data-v-73d3fb0a].el-input {
  max-width: 640px;
  width: 640px;
  display: -webkit-inline-box;
  display: -ms-inline-flexbox;
  display: inline-flex;
}
.el-checkbox {
  color: #666;
  font-weight: 500;
  font-size: 14px;
  position: relative;
  cursor: pointer;
  display: inline-block;
  white-space: nowrap;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
[data-v-73d3fb0a].el-checkbox {
  margin-left: 20px;
}
.el-checkbox__input {
  white-space: nowrap;
  cursor: pointer;
  outline: none;
  display: inline-block;
  line-height: 1;
  position: relative;
  vertical-align: middle;
}
.el-checkbox__label {
  display: inline-block;
  padding-left: 10px;
  line-height: 19px;
  font-size: 14px;
}
#app .el-checkbox__label {
  font-size: 12px;
  color: #333;
  font-weight: 400;
  width: 60px;
}
.el-checkbox__inner {
  display: inline-block;
  position: relative;
  border: 1px solid #dadde4;
  border-radius: 2px;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  width: 14px;
  height: 14px;
  background-color: #fff;
  z-index: 1;
  -webkit-transition: border-color 0.25s cubic-bezier(0.71, -0.46, 0.29, 1.46),
    background-color 0.25s cubic-bezier(0.71, -0.46, 0.29, 1.46);
  transition: border-color 0.25s cubic-bezier(0.71, -0.46, 0.29, 1.46),
    background-color 0.25s cubic-bezier(0.71, -0.46, 0.29, 1.46);
}
.el-checkbox__original {
  opacity: 0;
  outline: none;
  position: absolute;
  margin: 0;
  width: 0px;
  height: 0px;
  z-index: -1;
}
.el-input__inner {
  -webkit-appearance: none;
  background-color: #fff;
  background-image: none;
  border-radius: 2px;
  border: 1px solid #dadde4;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  color: #666;
  display: inline-block;
  font-size: inherit;
  height: 40px;
  line-height: 40px;
  outline: none;
  padding: 0 15px;
  -webkit-transition: border-color 0.2s cubic-bezier(0.645, 0.045, 0.355, 1);
  transition: border-color 0.2s cubic-bezier(0.645, 0.045, 0.355, 1);
  width: 100%;
}
.el-input-group > .el-input__inner {
  vertical-align: middle;
  display: table-cell;
}
.el-input-group--append .el-input__inner {
  border-top-right-radius: 0px;
  border-bottom-right-radius: 0px;
}
.el-input [data-v-73d3fb0a].el-input__inner {
  -webkit-box-flex: 1;
  -ms-flex: 1;
  flex: 1;
  height: 20px;
  line-height: 20px;
  padding: 10px 15px;
  -webkit-box-sizing: content-box;
  box-sizing: content-box;
}
.el-input-group__append,
.el-input-group__prepend {
  background-color: #f5f7fa;
  color: #909399;
  vertical-align: middle;
  display: table-cell;
  position: relative;
  border: 1px solid #dadde4;
  border-radius: 2px;
  padding: 0 20px;
  width: 1px;
  white-space: nowrap;
}
.el-input-group__append {
  border-left: 0;
}
.el-input-group--prepend .el-input__inner,
.el-input-group__append {
  border-top-left-radius: 0px;
  border-bottom-left-radius: 0px;
}
[data-v-73d3fb0a].el-input-group__append {
  background-color: #637cbc;
  border-color: #637cbc;
  color: #fff;
  padding: 0 40px;
  font-size: 22px;
  cursor: pointer;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  width: 103px;
}
[data-v-431171e6].category-item {
  margin-right: 17px;
  padding-bottom: 1px;
  line-height: 20px;
  border-bottom: 1.5px solid transparent;
  cursor: pointer;
}
[data-v-431171e6].category-item-active,
[data-v-431171e6].category-item:hover {
  border-color: #637cbc;
  color: #637cbc;
}
.el-dialog {
  position: relative;
  margin: 0 auto 50px;
  background: #fff;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 3px rgba(0, 0, 0, 0.3);
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.3);
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  width: 50%;
}
.el-dialog--center {
  text-align: center;
}
.el-dialog__header {
  padding: 20px;
  padding-bottom: 10px;
}
.el-dialog__title {
  line-height: 24px;
  font-size: 18px;
  color: #333;
}
.feedback-dialog .el-dialog__title {
  color: #333;
  font-size: 22px;
  font-weight: 600;
}
.el-dialog__headerbtn {
  position: absolute;
  top: 20px;
  right: 20px;
  padding: 0;
  background: transparent;
  border: none;
  outline: none;
  cursor: pointer;
  font-size: 16px;
}
.el-dialog__headerbtn .el-dialog__close {
  color: #909399;
}
.feedback-dialog .el-dialog__close {
  font-size: 24px;
}
.collect-dialog .el-dialog__header {
  padding: 0;
}
.login-dialog .el-dialog__body,
.login-dialog .el-dialog__header {
  padding: 0;
}
.wenshu-content h1[data-v-2da6a776]::before, .wenshu-content h2[data-v-2da6a776]::before {
    display: inline-block;
    content: "";
    width: 3px;
    height: 20px;
    margin-right: 14px;
    position: relative;
    top: 3px;
    background-color: #637cbc;
}
.text_wrap {
    margin-bottom: 20px;
    text-indent: 2em;
}
.sep-wrapper .sep-item::after {
    content: "|";
    color: #8b94aa;
    margin: 0 18px;
}

</style>
