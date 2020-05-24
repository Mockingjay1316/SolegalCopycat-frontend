<template>
  <div class="home">
    <div class="flex-col main">
      <div class="flex-col home-wrapper main-align-center cross-align-center">
        <div class="flex-col home">
          <div class="flex-col main">
            <div class="flex-col home-wrapper main-align-center cross-align-center" data-v-2b4bae82>
              <div class="flex-col home" data-v-2b4bae82>
                <a
                  class="logo-wrapper flex-row main-align-center router-link-exact-active router-link-active"
                  href="/"
                  data-v-2b4bae82
                >
                  <img
                    class="logo"
                    src="../assets/solegal_logo.png"
                    data-v-2b4bae82
                  />
                </a>
                <div class="flex-row main-align-center" style="margin-top: 40px;" data-v-2b4bae82>
                  <div data-v-2b4bae82 data-v-73d3fb0a>
                    <div
                      class="flex-row category-list cross-align-center"
                      data-v-73d3fb0a
                      data-v-08e47234
                    >
                      <span class="category-item category-item-active" data-v-08e47234>案例</span>
                      <span class="category-item" data-v-08e47234>法律法规</span>
                      <span class="category-item" data-v-08e47234>律师</span>
                      <span class="category-item" data-v-08e47234>律所</span>
                    </div>
                    <div class="search-box search-box-home" data-v-73d3fb0a>
                      <div class="el-input el-input-group el-input-group--append" data-v-73d3fb0a>
                        <input
                          class="el-input__inner"
                          autofocus="autofocus"
                          type="text"
                          maxlength="1000"
                          placeholder="请输入案情描述、关键词、案由、案号..."
                          v-model="input"
                          data-v-73d3fb0a
                        />
                        <div class="el-input-group__append" data-v-73d3fb0a @click="doSearch">
                          <i class="el-icon-search" data-v-73d3fb0a></i>
                        </div>
                      </div>
                      <!---->
                    </div>
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
export default {
  name: "Home",
  data() {
    return {
      input: ""
    };
  },
  methods: {
    doSearch(e) {
      console.log("click " + this.input, e);
      this.$router.push({ path: "/search", query: { key: this.input, page: 1 } });
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
.flex-1 {
  -webkit-box-flex: 1;
  -ms-flex: 1;
  flex: 1;
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
[data-v-02e0c782].close {
  position: absolute;
  top: 20px;
  right: 20px;
  color: #ccc;
}
.hot-item-law [data-v-02e0c782].icon {
  color: #f8a724;
  margin-left: 6px;
  font-size: 18px;
  line-height: 20px;
  position: relative;
  top: -1px;
}
.login-switch i[data-v-0a80d877] {
  cursor: pointer;
  font-size: 40px;
}
#app [class*=" el-icon-my"],
#app [class^="el-icon-my"] {
  font-family: iconfont !important;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
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
[data-v-2b4bae82].home {
  margin-top: 40px;
  -webkit-transition: margin 0.4s;
  transition: margin 0.4s;
}
/* @media screen and (max-height:1600px) */
[data-v-2b4bae82].home {
  margin-top: 290px;
}
/* @media screen and (max-height:1440px) */
[data-v-2b4bae82].home {
  margin-top: 140px;
}
[data-v-2b4bae82].logo-wrapper {
  cursor: auto;
}
.box-shadow {
  background: #fff;
  -webkit-box-shadow: 2px 2px 8px 0 rgba(0, 0, 0, 0.08);
  box-shadow: 2px 2px 8px 0px rgba(0, 0, 0, 0.08);
}
[data-v-2b4bae82].info-flow-wrapper {
  margin-top: 70px;
  margin-bottom: 100px;
}
[data-v-02e0c782].info-flow-wrapper {
  position: relative;
  width: 850px;
  color: #666;
  font-size: 14px;
  line-height: 24px;
}
.info-flow-wrapper [data-v-02e0c782].info-flow-list {
  width: 547px;
}
[data-v-02e0c782].hot-list-wrapper {
  margin-left: 35px;
  padding-right: 20px;
  padding-top: 20px;
  padding-bottom: 8px;
}
[data-v-02e0c782].hot-list {
  font-size: 14px;
  color: #333;
  line-height: 20px;
}
[data-v-02e0c782].hot-list-title {
  margin-top: 5px;
  margin-bottom: 13px;
  font-size: 16px;
  color: #333;
  font-weight: 600;
  line-height: 22px;
}
.one-line {
  white-space: nowrap;
  display: block;
}
.one-line,
.two-line {
  overflow: hidden;
  text-overflow: ellipsis;
}
.two-line {
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}
[data-v-02e0c782].hot-item-case {
  margin-bottom: 12px;
}
[data-v-02e0c782].hot-list-law {
  -ms-flex-wrap: wrap;
  flex-wrap: wrap;
}
[data-v-02e0c782].hot-item-law {
  width: 120px;
  line-height: 20px;
  margin-bottom: 10px;
}
.info-flow-wrapper [data-v-02e0c782].info-item {
  padding: 0 20px;
  width: 100%;
}
.info-flow-wrapper .info-item [data-v-02e0c782].info-item-inner {
  padding: 20px 0;
  border-bottom: 2px solid #f6f6f6;
}
.info-flow-wrapper :last-child.info-item [data-v-02e0c782].info-item-inner {
  border-bottom: none;
}
.info-flow-wrapper .info-item [data-v-02e0c782].title {
  font-size: 16px;
  color: #333;
  font-weight: 600;
  line-height: 24px;
  max-height: 48px;
}
.info-flow-wrapper .info-item [data-v-02e0c782].tag-list {
  margin-top: 10px;
  white-space: nowrap;
}
.info-flow-wrapper .info-item [data-v-02e0c782].tag {
  font-size: 13px;
  color: #666;
  line-height: 18px;
  overflow: hidden;
  text-overflow: ellipsis;
}
.info-flow-wrapper .info-item .tag + [data-v-02e0c782].tag {
  margin-left: 14px;
}
[data-v-08e47234].category-list {
  height: 40px;
  font-size: 14px;
  color: #666;
  position: relative;
  top: -5px;
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
.search-box-home + [data-v-73d3fb0a].suggestion {
  width: 606px;
  max-width: 606px;
}
.main-align-space-between {
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
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
.search-box-home [data-v-73d3fb0a].el-input {
  max-width: 710px;
  width: 710px;
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
.search-box-home .el-input [data-v-73d3fb0a].el-input__inner {
  padding: 13px 15px;
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
[data-v-08e47234].category-item {
  font-size: 16px;
  line-height: 27px;
  padding: 0 9px;
  border-radius: 5px;
  cursor: pointer;
  position: relative;
}
[data-v-08e47234].category-item-active {
  color: #fff;
  background: #637cbc;
}
.category-item + [data-v-08e47234].category-item {
  margin-left: 10px;
}
[data-v-2b4bae82].logo {
  height: 62px;
  width: auto;
}
[data-v-130acafa].headerbar {
  padding-bottom: 13px;
  -ms-flex-negative: 0;
  flex-shrink: 0;
  background-color: #fff;
  border-bottom: 1px solid #eaedf3;
  min-height: 50px;
}
[data-v-130acafa].headerbar-home {
  background: none;
  border-bottom: none;
  padding: 0 46px;
}
.cross-align-end {
  -webkit-box-align: end;
  -ms-flex-align: end;
  align-items: flex-end;
}
[data-v-130acafa].headerbar-right {
  position: relative;
  top: -2px;
}
.el-button {
  display: inline-block;
  line-height: 1;
  white-space: nowrap;
  cursor: pointer;
  background: #fff;
  border: 1px solid #dadde4;
  border-color: #dadde4;
  color: #666;
  -webkit-appearance: none;
  text-align: center;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  outline: none;
  margin: 0;
  -webkit-transition: 0.1s;
  transition: 0.1s;
  font-weight: 500;
  -moz-user-select: none;
  -webkit-user-select: none;
  -ms-user-select: none;
  padding: 12px 20px;
  font-size: 14px;
  border-radius: 2px;
}
.el-button--medium {
  padding: 10px 20px;
  font-size: 14px;
  border-radius: 2px;
}
.el-button--text {
  border-color: transparent;
  color: #637cbc;
  background: transparent;
  padding-left: 0px;
  padding-right: 0px;
}
[data-v-130acafa].el-button {
  font-size: 14px;
  color: #333;
  font-weight: 400;
}
[data-v-130acafa].sep {
  border-right: 1px solid #c2c2c2;
  margin: 0 10px;
  height: 23px;
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
.el-dialog--center .el-dialog__body {
  text-align: initial;
  padding: 25px 25px 30px;
}
.login-dialog .el-dialog__body,
.login-dialog .el-dialog__header {
  padding: 0;
}
.el-dialog__body {
  padding: 30px 20px;
  color: #666;
  font-size: 14px;
}
[data-v-0a80d877].login-inner {
  width: 300px;
  margin: 0 auto;
  text-align: center;
}
[data-v-0a80d877].hd {
  margin-top: 40px;
}
#qrcode_login_container {
  height: 370px;
  overflow: hidden;
}
[data-v-0a80d877].login-switch {
  position: absolute;
  bottom: 8px;
  right: 8px;
  width: 40px;
  height: 40px;
  line-height: 40px;
  color: #8b94aa;
  cursor: pointer;
}
[data-v-0a80d877].tab-list {
  font-size: 20px;
  color: #333;
}
[data-v-0a80d877].tab-item-title {
  padding-bottom: 4px;
  font-weight: 500;
  cursor: pointer;
}
.tab-item-active [data-v-0a80d877].tab-item-title {
  color: #637cbc;
  border-bottom: 1px solid #637cbc;
}
[data-v-0a80d877].logo {
  margin-top: 40px;
  margin-bottom: 10px;
  height: 35px;
  width: auto;
}
</style>
