<template>
  <div class="about">
    <h1>{{ this.$route.query.key }}</h1>
    <div class="flex-col" id="app">
      <div class="el-dialog__wrapper" style="display: none;" data-v-0a80d877>
        <div
          class="el-dialog el-dialog--center login-dialog"
          style="width: 360px; margin-top: 15vh;"
        >
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
              <a
                class="logo flex-row cross-align-center router-link-active"
                href="/"
                data-v-130acafa
              ></a>
              <div class="flex-col" data-v-130acafa>
                <div data-v-130acafa data-v-73d3fb0a>
                  <div
                    class="flex-row category-list cross-align-center"
                    data-v-73d3fb0a
                    data-v-431171e6
                  >
                    <span class="category-item category-item-active" data-v-431171e6>案例</span>
                    <span class="category-item" data-v-431171e6>法律法规</span>
                    <span class="category-item" data-v-431171e6>律师</span>
                    <span class="category-item" data-v-431171e6>律所</span>
                  </div>
                  <div class="search-box" data-v-73d3fb0a>
                    <div class="el-input el-input-group el-input-group--append" data-v-73d3fb0a>
                      <input
                        class="el-input__inner"
                        type="text"
                        maxlength="1000"
                        placeholder="请输入案情描述、关键词、案由、案号..."
                        v-bind:value="this.$route.query.key"
                        data-v-73d3fb0a
                      />
                      <div class="el-input-group__append" data-v-73d3fb0a>
                        <i class="el-icon-search" data-v-73d3fb0a></i>
                      </div>
                    </div>
                    <label class="el-checkbox" role="checkbox" data-v-73d3fb0a>
                      <span class="el-checkbox__input" aria-checked="mixed">
                        <span class="el-checkbox__inner"></span>
                        <input
                          class="el-checkbox__original"
                          aria-hidden="true"
                          type="checkbox"
                          value
                        />
                      </span>
                      <span class="el-checkbox__label">
                        精确搜索
                        <!---->
                      </span>
                    </label>
                  </div>
                  <div
                    class="flex-col suggestion box-shadow"
                    style="left: 134px; top: 82px; display: none;"
                    data-v-73d3fb0a
                  ></div>
                </div>
              </div>
            </div>
            <div class="flex-row headerbar-right cross-align-center" data-v-130acafa>
              <!---->
              <div class="flex-row user-zone cross-align-center" data-v-130acafa>
                <div data-v-130acafa>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="flex-col main">
        <div class="flex-col" style="margin-bottom: 60px;" data-v-0eb21d13>
          <div class="flex-col status-wrapper" data-v-0eb21d13>
            <div class="flex-row status cross-align-center" data-v-0eb21d13>
              <div class="flex-row cross-align-baseline inner" data-v-0eb21d13>
                <span class="text" data-v-0eb21d13>筛选条件:</span>
                <div class="flex-row filter-list flex-1 cross-align-center" data-v-0eb21d13>
                  <span class="filter-item" data-v-0eb21d13>
                    <div
                      tabindex="0"
                      class="el-popover el-popper filter-item-popper"
                      id="el-popover-5844"
                      role="tooltip"
                      aria-hidden="true"
                      style="display: none;"
                    >
                      <!---->
                      <div
                        class="flex-row main-align-center cross-align-center replace-tip"
                        data-v-0eb21d13
                      >
                        仍然搜索：
                        <span data-v-0eb21d13>{{this.$route.query.key}}</span>
                      </div>
                    </div>
                    <span
                      tabindex="0"
                      v-bind:title="this.$route.query.key"
                      class="el-tag el-tag--medium el-popover__reference"
                      aria-describedby="el-popover-5844"
                      data-v-0eb21d13
                    >
                      {{this.$route.query.key}}
                      <i class="el-tag__close el-icon-close"></i>
                    </span>
                  </span>
                </div>
              </div>
            </div>
            <div class="flex-row subtype-selection cross-align-start inner" data-v-0eb21d13>
              <span class="text" style="line-height: 40px;" data-v-0eb21d13>案例选择:</span>
              <div class="flex-1 el-tabs el-tabs--top" data-v-0eb21d13>
                <div class="el-tabs__header is-top">
                  <div class="el-tabs__nav-wrap is-top">
                    <div class="el-tabs__nav-scroll">
                      <div
                        class="el-tabs__nav is-top"
                        role="tablist"
                        style="transform: translateX(0px);"
                      >
                        <div
                          class="el-tabs__active-bar is-top"
                          style="width: 87px; transform: translateX(112px);"
                        ></div>
                        <div
                          tabindex="-1"
                          class="el-tabs__item is-top"
                          id="tab-authcase"
                          role="tab"
                          aria-controls="pane-authcase"
                        >
                          <span data-v-0eb21d13>权威案例(0)</span>
                        </div>
                        <div
                          tabindex="0"
                          class="el-tabs__item is-top is-active"
                          id="tab-case"
                          role="tab"
                          aria-selected="true"
                          aria-controls="pane-case"
                        >
                          <span data-v-0eb21d13>普通案例(163)</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="el-tabs__content">
                  <div
                    class="el-tab-pane"
                    id="pane-authcase"
                    role="tabpanel"
                    aria-hidden="true"
                    aria-labelledby="tab-authcase"
                    style="display: none;"
                    data-v-0eb21d13
                  ></div>
                  <div
                    class="el-tab-pane"
                    id="pane-case"
                    role="tabpanel"
                    aria-labelledby="tab-case"
                    data-v-0eb21d13
                  ></div>
                </div>
              </div>
            </div>
          </div>
          <div data-v-0eb21d13>
            <div class="flex-row inner" style="display: none;" data-v-0eb21d13 data-v-4da420ba>
              <div class="flex-col sidebar box-shadow" style="display: none;" data-v-4da420ba>
                <div
                  class="keyword-in-result el-input el-input--mini el-input--suffix"
                  data-v-4da420ba
                >
                  <!---->
                  <input
                    class="el-input__inner"
                    type="text"
                    placeholder="在结果中搜索"
                    autocomplete="off"
                  />
                  <!---->
                  <span class="el-input__suffix">
                    <span class="el-input__suffix-inner">
                      <i class="search-icon-btn el-icon-search el-input__icon" data-v-4da420ba></i>
                      <!---->
                    </span>
                    <!---->
                  </span>
                  <!---->
                </div>
              </div>
              <!---->
              <div
                class="flex-col no-data cross-align-center main-align-center"
                data-v-343c852c
                data-v-4da420ba
              >
                <img alt="还没有数据哦!" src="//static.milvai.cn/static/nodata.png" data-v-343c852c />
                <span class="no-data-desc" data-v-343c852c>还没有数据哦!</span>
              </div>
            </div>
            <div class="flex-row inner" data-v-0eb21d13 data-v-4da420ba>
              <div class="flex-col sidebar box-shadow" data-v-4da420ba>
                <div
                  class="keyword-in-result el-input el-input--mini el-input--suffix"
                  data-v-4da420ba
                >
                  <!---->
                  <input
                    class="el-input__inner"
                    type="text"
                    placeholder="在结果中搜索"
                    autocomplete="off"
                  />
                  <!---->
                  <span class="el-input__suffix">
                    <span class="el-input__suffix-inner">
                      <i class="search-icon-btn el-icon-search el-input__icon" data-v-4da420ba></i>
                      <!---->
                    </span>
                    <!---->
                  </span>
                  <!---->
                </div>
                <div class="flex-col sidebar-item" data-v-4da420ba>
                  <div class="flex-row sidebar-item-header cross-align-baseline" data-v-4da420ba>
                    <i class="sidebar-title-icon el-icon-my-aiyou" data-v-4da420ba></i>
                    <span class="sidebar-title" data-v-4da420ba>案件案由</span>
                  </div>
                  <div class="flex-row sidebar-item-content" data-v-4da420ba>
                    <div class="layer-wrapper" data-v-28ee65e2 data-v-4da420ba>
                      <div class="el-tree layer" role="tree" data-v-28ee65e2>
                        <div
                          tabindex="0"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">民事(110)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">刑事(46)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">行政(6)</span>
                          </div>
                          <!---->
                        </div>
                        <!---->
                        <div class="el-tree__drop-indicator" style="display: none;"></div>
                      </div>
                      <!---->
                    </div>
                  </div>
                </div>
                <div class="flex-col sidebar-item" data-v-4da420ba>
                  <div class="flex-row sidebar-item-header cross-align-baseline" data-v-4da420ba>
                    <i class="sidebar-title-icon el-icon-my-diyu" data-v-4da420ba></i>
                    <span class="sidebar-title" data-v-4da420ba>案件地域</span>
                  </div>
                  <div class="flex-row sidebar-item-content" data-v-4da420ba>
                    <div class="layer-wrapper" data-v-28ee65e2 data-v-4da420ba>
                      <div class="el-tree layer" role="tree" data-v-28ee65e2>
                        <div
                          tabindex="0"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">广东(35)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">北京(20)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">辽宁(11)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">河北(9)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">内蒙古(7)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">四川(7)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">重庆(6)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">浙江(5)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">山东(5)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">江苏(4)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">湖南(4)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">吉林(3)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">黑龙江(3)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">上海(3)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">河南(3)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">广西(3)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">贵州(3)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">陕西(3)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">天津(2)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">福建(2)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">湖北(2)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">最高人民法院(1)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">山西(1)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">江西(1)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">海南(1)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">青海(1)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">宁夏(1)</span>
                          </div>
                          <!---->
                        </div>
                        <!---->
                        <div class="el-tree__drop-indicator" style="display: none;"></div>
                      </div>
                      <!---->
                    </div>
                  </div>
                </div>
                <div class="flex-col sidebar-item" data-v-4da420ba>
                  <div class="flex-row sidebar-item-header cross-align-baseline" data-v-4da420ba>
                    <i class="sidebar-title-icon el-icon-my-cengji" data-v-4da420ba></i>
                    <span class="sidebar-title" data-v-4da420ba>法院层级</span>
                  </div>
                  <div class="flex-row sidebar-item-content" data-v-4da420ba>
                    <div class="layer-wrapper" data-v-28ee65e2 data-v-4da420ba>
                      <div class="el-tree layer" role="tree" data-v-28ee65e2>
                        <div
                          tabindex="0"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">最高人民法院(1)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">高级人民法院(10)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">中级人民法院(40)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">基层人民法院(95)</span>
                          </div>
                          <!---->
                        </div>
                        <!---->
                        <div class="el-tree__drop-indicator" style="display: none;"></div>
                      </div>
                      <!---->
                    </div>
                  </div>
                </div>
                <div class="flex-col sidebar-item" data-v-4da420ba>
                  <div class="flex-row sidebar-item-header cross-align-baseline" data-v-4da420ba>
                    <i class="sidebar-title-icon el-icon-my-nianfen" data-v-4da420ba></i>
                    <span class="sidebar-title" data-v-4da420ba>文书年份</span>
                  </div>
                  <div class="flex-row sidebar-item-content" data-v-4da420ba>
                    <div class="layer-wrapper" data-v-28ee65e2 data-v-4da420ba>
                      <div class="el-tree layer" role="tree" data-v-28ee65e2>
                        <div
                          tabindex="0"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">2018年(24)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">2017年(46)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">2016年(34)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">2015年(29)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">2014年(21)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">2013年(5)</span>
                          </div>
                          <!---->
                        </div>
                        <!---->
                        <div class="el-tree__drop-indicator" style="display: none;"></div>
                      </div>
                      <!---->
                    </div>
                  </div>
                </div>
                <div class="flex-col sidebar-item" data-v-4da420ba>
                  <div class="flex-row sidebar-item-header cross-align-baseline" data-v-4da420ba>
                    <i class="sidebar-title-icon el-icon-my-chengxu" data-v-4da420ba></i>
                    <span class="sidebar-title" data-v-4da420ba>审判程序</span>
                  </div>
                  <div class="flex-row sidebar-item-content" data-v-4da420ba>
                    <div class="layer-wrapper" data-v-28ee65e2 data-v-4da420ba>
                      <div class="el-tree layer" role="tree" data-v-28ee65e2>
                        <div
                          tabindex="0"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">一审案件(120)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">二审案件(40)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">再审案件(1)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">其他(2)</span>
                          </div>
                          <!---->
                        </div>
                        <!---->
                        <div class="el-tree__drop-indicator" style="display: none;"></div>
                      </div>
                      <!---->
                    </div>
                  </div>
                </div>
                <div class="flex-col sidebar-item" data-v-4da420ba>
                  <div class="flex-row sidebar-item-header cross-align-baseline" data-v-4da420ba>
                    <i class="sidebar-title-icon el-icon-my-wenshuleixing" data-v-4da420ba></i>
                    <span class="sidebar-title" data-v-4da420ba>文书类型</span>
                  </div>
                  <div class="flex-row sidebar-item-content" data-v-4da420ba>
                    <div class="layer-wrapper" data-v-28ee65e2 data-v-4da420ba>
                      <div class="el-tree layer" role="tree" data-v-28ee65e2>
                        <div
                          tabindex="0"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">判决书(157)</span>
                          </div>
                          <!---->
                        </div>
                        <div
                          tabindex="-1"
                          class="el-tree-node is-focusable"
                          role="treeitem"
                          aria-disabled
                          draggable="false"
                        >
                          <div class="el-tree-node__content" style="padding-left: 0px;">
                            <span class="el-tree-node__expand-icon el-icon-caret-right is-leaf"></span>
                            <!---->
                            <!---->
                            <span class="el-tree-node__label">裁定书(5)</span>
                          </div>
                          <!---->
                        </div>
                        <!---->
                        <div class="el-tree__drop-indicator" style="display: none;"></div>
                      </div>
                      <!---->
                    </div>
                  </div>
                </div>
              </div>
              <div class="flex-col flex-1 result" data-v-4da420ba>
                <div
                  class="flex-row toolbar box-shadow main-align-space-between cross-align-center"
                  data-v-4da420ba
                >
                  <div class="flex-row cross-align-center toolbar-left" data-v-4da420ba>
                    <!---->
                  </div>
                  <div class="flex-row" data-v-4da420ba>
                    <span data-v-4da420ba>共搜索到{{totalItemNum}}条内容</span>
                  </div>
                </div>
                <!-- insert here -->
                <SearchItem
                  v-for="item in itemData"
                  v-bind:key="item.id"
                  v-bind:title="item.title"
                  v-bind:content="item.content"
                ></SearchItem>
                <div class="flex-row pagination main-align-center box-shadow" data-v-4da420ba>
                  <div class="el-pagination is-background" data-v-4da420ba>
                    <span style="color: rgb(102, 102, 102);" data-v-4da420ba>共 {{totalItemNum}} 条</span>
                    <button disabled="disabled" class="btn-prev" type="button">
                      <i class="el-icon el-icon-arrow-left"></i>
                    </button>
                    <ul class="el-pager">
                      <li class="number active">1</li>
                      <!---->
                      <li class="number">2</li>
                      <li class="number">3</li>
                      <li class="number">4</li>
                      <li class="number">5</li>
                      <li class="number">6</li>
                      <li class="el-icon more btn-quicknext el-icon-more"></li>
                      <li class="number">9</li>
                    </ul>
                    <button class="btn-next" type="button">
                      <i class="el-icon el-icon-arrow-right"></i>
                    </button>
                  </div>
                </div>
              </div>
              <!---->
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SearchItem from '@/components/SearchItem.vue'
import axios from 'axios'

export default {
  name: "Search",
  data: function() { 
    return {
      newTodoText: '',
      sitems: [
        {
          id: 1,
          title: '1',
          content: '1',
        },
        {
          id: 2,
          title: '2',
          content: '2',
        },
        {
          id: 3,
          title: '3',
          content: '3',
        }
      ],
      nextTodoId: 4,
      totalItemNum: 0,
      i: 0,
      itemData: null
    }
  },
  mounted: function() {
    console.log("get " + this.$route.query.key);
    axios
      .get('http://127.0.0.1:8010/search/common/?keyword='+this.$route.query.key)
      .then(response => {
        this.itemData = new Array();
        console.log(response.data.result[0]);
        for (var i = 0;i < response.data.result.length; i++) {
          this.itemData.push({
            id: i,
            title: response.data.result[i].AH,
            content: response.data.result[i].QW.substring(0,200)
          })
        }
      })
      .catch(error => console.log(error))
  },
  components: {
    SearchItem
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
.flex-col, .flex-row {
	display: -webkit-box;
	display: -ms-flexbox;
	display: flex;
	-webkit-box-direction: normal;
}
#app {
	min-height: 100%;
}
body {
	font-family: -apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Helvetica,PingFang SC,Hiragino Sans GB,Microsoft YaHei,SimSun,sans-serif;
	-webkit-font-smoothing: antialiased;
	line-height: 1.5;
	-webkit-tap-highlight-color: rgba(0, 0, 0, 0);
	overflow: auto;
}
html {
	font-size: 37.5px;
}
body, html {
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
.main-align-space-between {
	-webkit-box-pack: justify;
	-ms-flex-pack: justify;
	justify-content: space-between;
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
	-webkit-transition: all .5s ease-in-out;
	transition: all .5s ease-in-out;
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
	-webkit-box-shadow: 0 2px 4px 0 hsla(0,0%,85.1%,.5);
	box-shadow: 0px 2px 4px 0px hsla(0, 0%, 85%, 0.5);
	padding: 10px;
	border-radius: 4px;
}
i {
	font-style: normal;
}
li {
	list-style: none;
}
[class*=' el-icon-'], [class^=el-icon-] {
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
.btn-hover i {
	margin-right: 5px;
}
.toolbar .btn-hover i[data-v-c001cdde] {
	font-size: 14px;
}
.toolbar .btn-hover [data-v-c001cdde].lishen-arrow {
	font-size: 12px;
	color: #8b94aa;
	position: relative;
	top: 1px;
	-webkit-transform: scale(0.8);
	transform: scale(0.8);
}
.sidebar [data-v-4da420ba].sidebar-title-icon {
	margin-right: 10px;
	font-size: 20px;
	color: #637cbc;
}
#app [class*=' el-icon-my'], #app [class^=el-icon-my] {
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
[data-v-0eb21d13].status-wrapper {
	padding-left: 30px;
	padding-right: 30px;
	background: #f9fbfb;
}
.cross-align-start {
	-webkit-box-align: start;
	-ms-flex-align: start;
	align-items: flex-start;
}
.cross-align-baseline {
	-webkit-box-align: baseline;
	-ms-flex-align: baseline;
	align-items: baseline;
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
[data-v-4da420ba].inner {
	margin-top: 15px;
}
.box-shadow {
	background: #fff;
	-webkit-box-shadow: 2px 2px 8px 0 rgba(0,0,0,.08);
	box-shadow: 2px 2px 8px 0px rgba(0,0,0,0.08);
}
[data-v-4da420ba].sidebar {
	color: #333;
	margin-right: 25px;
	width: 280px;
	background: #fff;
	padding: 20px;
	-ms-flex-item-align: start;
	align-self: flex-start;
}
[data-v-4da420ba].toolbar {
	height: 60px;
	margin-bottom: 16px;
	padding: 0 20px;
	color: #666;
}
[data-v-4da420ba].result-item {
	position: relative;
	background: #fff;
}
.result-item + [data-v-4da420ba].result-item {
	margin-top: 18px;
}
[data-v-4da420ba].pagination {
	margin-top: 10px;
	background: #fff;
	padding: 10px 20px;
}
.el-pagination {
	white-space: nowrap;
	padding: 2px 5px;
	color: #333;
	font-weight: 700;
}
.el-pagination button, .el-pagination span:not([class*=suffix]) {
	display: inline-block;
	font-size: 13px;
	min-width: 35.5px;
	height: 28px;
	line-height: 28px;
	vertical-align: top;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}
.el-pagination button {
	border: none;
	padding: 0 6px;
	background: transparent;
}
.el-pagination .btn-next, .el-pagination .btn-prev {
	background: 50% no-repeat;
	background-size: 16px;
	background-color: #fff;
	cursor: pointer;
	margin: 0;
	color: #333;
}
.el-pagination .btn-prev {
	padding-right: 12px;
}
.el-pagination button:disabled {
	color: #c0c4cc;
	background-color: #fff;
	cursor: not-allowed;
}
.el-pagination .btn-next {
	padding-left: 12px;
}
.el-pager li.active {
	color: #637cbc;
	cursor: default;
}
.el-pager li.active + li {
	border-left: 0;
}
.el-pager li {
	padding: 0 4px;
	background: #fff;
	vertical-align: top;
	display: inline-block;
	font-size: 13px;
	min-width: 35.5px;
	height: 28px;
	line-height: 28px;
	cursor: pointer;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
	text-align: center;
	margin: 0;
}
.el-pager li.btn-quicknext, .el-pager li.btn-quickprev {
	line-height: 28px;
	color: #333;
}
.el-pagination.is-background .btn-next, .el-pagination.is-background .btn-prev, .el-pagination.is-background .el-pager li {
	margin: 0 5px;
	background-color: #f4f4f5;
	color: #666;
	min-width: 30px;
	border-radius: 2px;
}
.el-pagination.is-background .btn-next, .el-pagination.is-background .btn-prev {
	padding: 0;
}
.el-pagination.is-background :disabled.btn-next, .el-pagination.is-background :disabled.btn-prev {
	color: #c0c4cc;
}
.el-pager {
	-webkit-user-select: none;
	-moz-user-select: none;
	-ms-user-select: none;
	user-select: none;
	list-style: none;
	display: inline-block;
	vertical-align: top;
	font-size: 0px;
	padding: 0;
	margin: 0;
}
.el-pagination .btn-next .el-icon, .el-pagination .btn-prev .el-icon {
	display: block;
	font-size: 12px;
	font-weight: 700;
}
.el-pagination.is-background .el-pager li:not(.disabled).active {
	background-color: #637cbc;
	color: #fff;
}
[data-v-c001cdde].item-inner {
	padding: 0 20px;
	width: 100%;
}
[data-v-c001cdde].toolbar {
	background: #fbfbfb;
	height: 40px;
	border-top: 1px solid #eaedf3;
}
.toolbar [data-v-c001cdde].btn-hover {
	height: 20px;
	line-height: 20px;
	-webkit-box-align: center;
	-ms-flex-align: center;
	align-items: center;
}
.toolbar .btn-hover + [data-v-c001cdde].btn-hover {
	margin-left: 35px;
}
.filter-item-popper {
	padding: 0 !important;
	min-width: auto !important;
	margin-top: 5px !important;
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
	-webkit-box-shadow: 0 2px 12px 0 rgba(0,0,0,.1);
	box-shadow: 0px 2px 12px 0px rgba(0,0,0,0.1);
}
.no-arrow.el-popper {
	margin-top: 0px !important;
}
.lishen-popper.el-popper {
	padding: 0;
}
[data-v-c001cdde].lishen-label {
	margin-right: 6px;
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
[data-v-5ab240b0].step-icon, [data-v-5ab240b0].step-line-inner {
	-webkit-transition: .15s ease-out;
	transition: .15s ease-out;
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
[data-v-c001cdde].wenshu-header {
	margin-top: 22px;
}
[data-v-c001cdde].wenshu-info {
	margin-top: 9px;
	line-height: 1;
}
[data-v-c001cdde].abstract {
	padding-bottom: 0px !important;
}
#app .abstract {
	font-size: 15px;
	line-height: 23px;
	color: #333;
	padding: 12px 0;
}
em {
	color: #c00;
	font-style: normal;
}
[data-v-6856ea31].sep-offset-left {
	margin-left: -0.5em;
}
[data-v-c001cdde].wenshu-title {
	color: #637cbc;
	font-size: 20px;
	font-weight: 400;
	line-height: 28px;
}
[data-v-4da420ba].toolbar-left {
	font-size: 16px;
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
	-webkit-transition: .1s;
	transition: .1s;
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
.toolbar-left [data-v-4da420ba].el-button {
	font-size: 16px;
	font-weight: 400;
}
.toolbar-left [data-v-4da420ba]:not(.is-disabled).el-button {
	color: #666;
}
.el-input {
	position: relative;
	font-size: 14px;
	display: inline-block;
	width: 100%;
}
.el-input--mini {
	font-size: 12px;
}
[data-v-4da420ba].keyword-in-result {
	margin-bottom: 10px;
	width: 238px;
}
.sidebar .sidebar-item + .sidebar-item [data-v-4da420ba].sidebar-item-header {
	margin-top: 15px;
}
[data-v-4da420ba].sidebar-item-content {
	margin-top: 4px;
	margin-left: -3px;
}
[data-v-28ee65e2].layer-wrapper {
	width: 100%;
	max-height: 260px;
	overflow-y: auto;
}
.el-tree {
	position: relative;
	cursor: default;
	background: #fff;
	color: #666;
}
[data-v-28ee65e2].layer {
	width: 100%;
}
.el-tree-node {
	white-space: nowrap;
	outline: none;
}
#app .el-tree-node {
	white-space: normal;
}
.el-tree__drop-indicator {
	position: absolute;
	left: 0px;
	right: 0px;
	height: 1px;
	background-color: #637cbc;
}
.el-tree-node__content {
	display: -webkit-box;
	display: -ms-flexbox;
	display: flex;
	-webkit-box-align: center;
	-ms-flex-align: center;
	align-items: center;
	height: 26px;
	cursor: pointer;
}
#app .el-tree-node__content {
	height: auto;
}
.el-tree-node__expand-icon {
	cursor: pointer;
	color: #c0c4cc;
	font-size: 12px;
	-webkit-transform: rotate(0deg);
	transform: rotate(0deg);
	-webkit-transition: -webkit-transform .3s ease-in-out;
	transition: -webkit-transform .3s ease-in-out;
	transition: transform .3s ease-in-out;
	transition: transform .3s ease-in-out,-webkit-transform .3s ease-in-out;
}
.el-tree-node__content > .el-tree-node__expand-icon {
	padding: 6px;
}
.el-tree-node__expand-icon.is-leaf {
	color: transparent;
	cursor: default;
}
.el-tree-node__label {
	font-size: 14px;
}
.sidebar [data-v-4da420ba].sidebar-title {
	font-size: 18px;
	color: #637cbc;
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
	-webkit-transition: border-color .2s cubic-bezier(.645,.045,.355,1);
	transition: border-color .2s cubic-bezier(.645,.045,.355,1);
	width: 100%;
}
.el-input--suffix .el-input__inner {
	padding-right: 30px;
}
.el-input--mini .el-input__inner {
	height: 28px;
	line-height: 28px;
}
.el-input__suffix {
	position: absolute;
	height: 100%;
	right: 5px;
	top: 0px;
	text-align: center;
	color: #c0c4cc;
	-webkit-transition: all .3s;
	transition: all .3s;
	pointer-events: none;
}
.el-input__suffix-inner {
	pointer-events: all;
}
.el-input__icon, .el-input__prefix {
	height: 100%;
	text-align: center;
	-webkit-transition: all .3s;
	transition: all .3s;
}
.el-input__icon {
	width: 25px;
	line-height: 40px;
}
.el-input--mini .el-input__icon {
	line-height: 28px;
}
[data-v-4da420ba].search-icon-btn {
	cursor: pointer;
}
[data-v-343c852c].no-data {
	width: 100%;
}
[data-v-4da420ba].no-data {
	height: 400px;
}
img[data-v-343c852c] {
	width: 170px;
	height: auto;
}
[data-v-343c852c].no-data-desc {
	margin-top: 10px;
	font-size: 16px;
	color: #8b94aa;
}
[data-v-0eb21d13].status {
	padding-top: 10px;
	color: #666;
}
[data-v-0eb21d13].text {
	width: 75px;
	font-weight: 400;
}
.el-tabs__header {
	padding: 0;
	position: relative;
	margin: 0 0 15px;
}
.subtype-selection .el-tabs__header {
	margin-bottom: 0px;
}
.el-tabs__content {
	overflow: hidden;
	position: relative;
}
.el-tabs__nav-wrap {
	overflow: hidden;
	margin-bottom: -1px;
	position: relative;
}
.el-tabs__nav-scroll {
	overflow: hidden;
}
.el-tabs__nav {
	white-space: nowrap;
	position: relative;
	-webkit-transition: -webkit-transform .3s;
	transition: -webkit-transform .3s;
	transition: transform .3s;
	transition: transform .3s,-webkit-transform .3s;
	float: left;
	z-index: 2;
}
.el-tabs__active-bar {
	position: absolute;
	bottom: 0px;
	left: 0px;
	height: 2px;
	background-color: #637cbc;
	z-index: 1;
	-webkit-transition: -webkit-transform .3s cubic-bezier(.645,.045,.355,1);
	transition: -webkit-transform .3s cubic-bezier(.645,.045,.355,1);
	transition: transform .3s cubic-bezier(.645,.045,.355,1);
	transition: transform .3s cubic-bezier(.645,.045,.355,1),-webkit-transform .3s cubic-bezier(.645,.045,.355,1);
	list-style: none;
}
.el-tabs__item {
	padding: 0 20px;
	height: 40px;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
	line-height: 40px;
	display: inline-block;
	list-style: none;
	font-size: 14px;
	font-weight: 500;
	color: #333;
	position: relative;
}
.el-tabs--bottom :nth-child(2).el-tabs__item.is-bottom, .el-tabs--bottom :nth-child(2).el-tabs__item.is-top, .el-tabs--top :nth-child(2).el-tabs__item.is-bottom, .el-tabs--top :nth-child(2).el-tabs__item.is-top {
	padding-left: 0px;
}
.el-tabs__item.is-active {
	color: #637cbc;
}
.el-tabs--bottom :last-child.el-tabs__item.is-bottom, .el-tabs--bottom :last-child.el-tabs__item.is-top, .el-tabs--top :last-child.el-tabs__item.is-bottom, .el-tabs--top :last-child.el-tabs__item.is-top {
	padding-right: 0px;
}
[data-v-0eb21d13].filter-list {
	-ms-flex-wrap: wrap;
	flex-wrap: wrap;
}
[data-v-0eb21d13].filter-item {
	margin-top: 5px;
	margin-bottom: 5px;
}
.el-select-dropdown__list, .el-tag {
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}
.el-tag {
	background-color: rgba(99, 124, 188, 0.1);
	display: inline-block;
	padding: 0 10px;
	height: 32px;
	line-height: 30px;
	font-size: 12px;
	color: #637cbc;
	border-radius: 4px;
	border: 1px solid rgba(99,124,188,.2);
	white-space: nowrap;
}
.el-tag--medium {
	height: 28px;
	line-height: 26px;
}
#app .el-tag {
	border-color: transparent;
}
.el-tag .el-icon-close {
	border-radius: 50%;
	text-align: center;
	position: relative;
	cursor: pointer;
	font-size: 12px;
	height: 16px;
	width: 16px;
	line-height: 16px;
	vertical-align: middle;
	top: -1px;
	right: -5px;
	color: #637cbc;
}
.el-tag--medium .el-icon-close {
	-webkit-transform: scale(0.8);
	transform: scale(0.8);
}
[data-v-0eb21d13].replace-tip {
	font-size: 12px;
	vertical-align: baseline;
	height: 40px;
	padding: 0 20px;
}
.replace-tip span[data-v-0eb21d13] {
	cursor: pointer;
	color: #637cbc;
	text-decoration: underline;
}
[data-v-130acafa].headerbar {
	padding-bottom: 13px;
	-ms-flex-negative: 0;
	flex-shrink: 0;
	background-color: #fff;
	border-bottom: 1px solid #eaedf3;
	min-height: 50px;
}
[data-v-130acafa].headerbar-right {
	position: relative;
	top: -2px;
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
[data-v-130acafa].logo {
	width: 134px;
	height: 60px;
	background-image: url("../assets/solegal_logo.png");
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
	-webkit-transition: border-color .25s cubic-bezier(.71,-.46,.29,1.46),background-color .25s cubic-bezier(.71,-.46,.29,1.46);
	transition: border-color .25s cubic-bezier(.71,-.46,.29,1.46),background-color .25s cubic-bezier(.71,-.46,.29,1.46);
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
.el-input-group__append, .el-input-group__prepend {
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
.el-input-group--prepend .el-input__inner, .el-input-group__append {
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
[data-v-431171e6].category-item-active, [data-v-431171e6].category-item:hover {
	border-color: #637cbc;
	color: #637cbc;
}
.el-dialog {
	position: relative;
	margin: 0 auto 50px;
	background: #fff;
	border-radius: 2px;
	-webkit-box-shadow: 0 1px 3px rgba(0,0,0,.3);
	box-shadow: 0px 1px 3px rgba(0,0,0,0.3);
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
.login-dialog .el-dialog__body, .login-dialog .el-dialog__header {
	padding: 0;
}

</style>