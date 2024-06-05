<template>
  <div id="app">
    <router-view v-if="isRouterAlive" />
  </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  name: 'App',
  computed: {
    ...mapState({
      isRouterAlive: state => state.common.isRouterAlive
    })
  }
}
</script>

<style>
  .el-dropdown-menu{
    background-color: #111113;
    color: white;
    margin: 1px solid #2a2a2e;
}

  .el-dropdown-menu__item{
    color: white;
  }

  .mobile-menu[data-v-b68dd620]{
    background-color: #111113;
  }

  .menu-main.el-menu[data-v-925fb65c]{
    background-color: #111113;
    color: white;
  }
  .el-menu{
    background-color: #111113;
  }
  .el-menu-item{
    color: white;
    background-color: #18181b;
  }

  #HomeCard .head-title[data-v-07312b9e]{
    color: white;
  }
  .el-message-box{
    background-color: #111113;
    color: white;
  }
  .el-button--default{
    background-color: #000;
    color:white;
  }
  .el-message-box__title{
    color: white;
  }
  .hamburger-container[data-v-0885fc76]{
    background-color: #000;
    color:white;
  }
  .left-menu.el-menu .el-submenu .el-submenu__title:hover{
    background-color: #111113;
  }
  .el-dialog__wrapper{
    background-color: #000;
    color:white;
  }
  .el-dialog__header{
    background-color: #111113;
    color:white;
  }
  .el-dialog__wrapper[data-v-9a0d807c] .el-dialog__body .tree-table .transition-box{
    background-color: #111113;
    color:white;
  }
  .el-dialog__wrapper[data-v-9a0d807c] .el-dialog__body .tree-table .mini{
    background-color: #111113;
    color:white;
  }
  .el-dialog__wrapper[data-v-2fb85988] .el-dialog__body .tree-table .right{
    background-color: #111113;
    color:white;
  }
  .dialog[data-v-6b5dcbfb] .el-dialog__footer{
    border-top: 1px solid #dee2e6;
    background-color: #111113;
    color:white;
  }
  .filter-field[data-v-243c7ff8] .el-cascader .el-input--suffix .el-input__inner {
    background-color: #111113;
    border: 1px solid #2a2a2e;
    color: white;
  }
  .el-table thead{
    background-color: #000 !important;
    color: white !important;
  }
  .el-table th, .el-table tr{
    background-color: #111113;
    color:white !important;
  }
  .el-data-table[data-v-3d11e000] .el-table td{
    background-color: #18181b;
    color:white !important;
  }
  .label-button[data-v-1e15d7b1] {
    background-color: #3c3f43;
    color:white;
    border: none !important;
  }
  .dialog-footer[data-v-6b5dcbfb] button.el-button {
    background-color: #111113;
    color:white;
  }
  .el-pagination .el-select .el-input .el-input__inner{
    background-color: #111113;
    color:white;
    border: 1px solid #2a2a2e !important;
  }
  .el-pagination.is-background .btn-prev:disabled{
    background-color: #18181b;
    border: 1px solid #2a2a2e;
    color: white;
  }
  .el-pagination.is-background .btn-next:disabled{
    background-color: #18181b;
    border: 1px solid #2a2a2e;
    color: white;
  }
  .el-pagination.is-background .el-pager li:not(.disabled).active {
    background-color: #18181b !important;
    border: 1px solid #fbbf24;
    color: #fbbf24 !important;
  }
  .el-card{
    border: 1px solid #2a2a2e !important;
  }
  .el-table--border{
    border: 1px solid #2a2a2e !important;
  }
  .dialog[data-v-6b5dcbfb] .el-dialog__body:has(.el-table) {
    background: #18181b !important;
  }
  .el-dialog__title {
    line-height: 24px;
    font-size: 18px;
    color: white !important;
  }
  .el-alert--success.is-light {
    background-color: #18181b !important;
    border: 1px solid #2a2a2e !important;
    color: #fbbf24 !important;
  }
  .el-alert--success.is-light .el-alert__description {
    color: #fbbf24 !important;
  }
  .el-link.el-link--info {
    color: #fbbf24 !important;
  }
  .left-menu.el-menu .el-menu-item:hover, .left-menu.el-menu .el-submenu-sidebar .el-menu-item:hover {
    background-color: #2a2a2e !important;
    list-style-type: disc;
  }
  td .el-button--primary.is-disabled {
    background-color: #fbbf24 !important;
  }
  .el-textarea__inner {
    display: block;
    resize: vertical;
    padding: 5px 15px;
    line-height: 1.5;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    width: 100%;
    font-size: inherit;
    color: #fff !important;
    background-color: #606266 !important;
    background-image: none;
    border: 1px solid #fbbf24 !important;
    border-radius: 4px;
    -webkit-transition: border-color .2s cubic-bezier(.645,.045,.355,1);
    transition: border-color .2s cubic-bezier(.645,.045,.355,1);
  }
  .el-switch.is-checked .el-switch__core {
    border-color: #fbbf24 !important;
    background-color: #fbbf24 !important;
  }
  .el-button--primary.is-disabled, .el-button--primary.is-disabled:active, .el-button--primary.is-disabled:focus, .el-button--primary:hover {
    background-color: #fbbf24 !important;
    border-color: #fbbf24 !important;
  }
  .el-dropdown-menu {
    position: absolute;
    top: 0;
    left: 0;
    padding: 10px 0;
    margin: 5px 0;
    background-color: #18181b !important;
    border: 1px solid #18181b !important;
    border-radius: 4px;
    box-shadow: 0 2px 12px 0 rgba(0, 0, 0, .1);
  }
  .el-dropdown-menu__item {
    list-style: none;
    line-height: 36px;
    padding: 0 20px;
    margin: 0;
    font-size: 13px;
    color: #fbbf24 !important;
    cursor: pointer;
    outline: 0;
  }
  .el-dropdown-menu__item--divided {
    position: relative;
    margin-top: 6px;
    border-top: 1px solid #2a2a2e !important;
  }
  .el-dropdown-menu__item--divided:before {
    content: '';
    height: 6px;
    display: block;
    margin: 0 -20px;
    background-color: #2a2a2e !important;
  }
  [data-v-0885fc76] .el-badge__content--primary {
    background-color: #fbbf24 !important;
  }
  [data-v-0885fc76] .el-badge__content {
    color: #fff !important;
  }
  .el-message-box {
    display: inline-block;
    width: 420px;
    padding-bottom: 10px;
    vertical-align: middle;
    background-color: #2a2a2e !important;
    border-radius: 4px;
    border: 1px solid #2d2d31 !important;
    font-size: 18px;
    -webkit-box-shadow: 0 2px 12px 0 rgba(0, 0, 0, .1);
    box-shadow: 0 2px 12px 0 rgba(0, 0, 0, .1);
    text-align: left;
    overflow: hidden;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
  }
  .el-message-box__title {
    padding-left: 0;
    margin-bottom: 0;
    font-size: 18px;
    line-height: 1;
    color: #fff !important;
  }
  .el-message-box__message p {
    margin: 0;
    line-height: 24px;
    color: #fff;
  }
  .el-button--danger {
    color: #FFF;
    background-color: #ff0000 !important;
    border-color: #ff0000 !important;
  }
  canvas {
    display: inline-block;
    color: #fff !important;
  }
  .el-button.is-disabled, .el-button.is-disabled:focus, .el-button.is-disabled:hover {
    color: #C0C4CC;
    cursor: not-allowed;
    background-image: none;
    background-color: #FFF;
    border-color: #fbbf24 !important;
  }
  .el-popover {
    position: absolute;
    background: #18181b !important;
    min-width: 200px !important;
    border: 1px solid #2d2d31 !important;
    padding: 12px;
    z-index: 2000;
    color: #fff !important;
    line-height: 1.4;
    text-align: justify;
    font-size: 13px;
    word-break: break-all;
  }
  .el-menu-item.is-active[data-v-925fb65c] {
    font-weight: bold;
    color: #fbbf24 !important;
    background-color: #000;
    border-left: 4px solid var(--menu-text-active);
  }
  .el-menu-item {
    font-size: 13px;
    color: #fff !important;
    padding: 0 20px;
    cursor: pointer;
    -webkit-transition: border-color .3s, background-color .3s, color .3s;
    transition: border-color .3s, background-color .3s, color .3s;
    box-sizing: border-box;
  }
  .el-tabs__nav-wrap::after {
    content: "";
    position: absolute;
    left: 0;
    bottom: 0;
    width: 100%;
    height: 2px;
    background-color: #fff !important;
    z-index: 1;
  }
  .el-tabs__active-bar {
    position: absolute;
    bottom: 0;
    left: 0;
    height: 2px;
    background-color: #fbbf24 !important;
    z-index: 1;
    -webkit-transition: -webkit-transform .3s cubic-bezier(.645,.045,.355,1);
    transition: -webkit-transform .3s cubic-bezier(.645,.045,.355,1);
    transition: transform .3s cubic-bezier(.645,.045,.355,1);
    transition: transform .3s cubic-bezier(.645,.045,.355,1), -webkit-transform .3s cubic-bezier(.645,.045,.355,1);
    list-style: none;
  }
  .wrapper-content[data-v-ecdb7b12] .el-button--primary {
    background-color: #fbbf24 !important;
    border: 1px solid #fbbf24 !important;
  }
  .el-dropdown-menu__item:focus, .el-dropdown-menu__item:not(.is-disabled):hover {
    background-color: #3c3f43 !important;
    color: inherit;
  }
  .el-card.info .el-card__header {
    background-color: #fbbf24 !important;
    border: 1px solid #fbbf24 !important;
  }
  .el-cascader-menu__list {
    position: relative;
    min-height: 100%;
    margin: 0;
    padding: 6px 0;
    list-style: none;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    background-color: #18181b !important;
    color: #FFF;
    border: 1px solid #2a2a2e !important;
  }
  .el-cascader-menu__wrap {
    height: 204px;
    border: 1px solid #2a2a2e !important;
  }
  .el-select-dropdown {
    position: absolute;
    z-index: 1001;
    border: 1px solid #2a2a2e !important;
    border-radius: 4px;
    background-color: #18181b !important;
    -webkit-box-shadow: 0 2px 12px 0 rgba(0, 0, 0, .1);
    box-shadow: 0 2px 12px 0 rgba(0, 0, 0, .1);
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    margin: 5px 0;
    color: #fff !important;
  }
  .el-dialog .el-dialog__body {
    max-height: 80vh;
    overflow: auto;
    padding: 30px;
    background-color: #18181b !important;
    color: #fff;
  }
  .el-checkbox__input.is-checked .el-checkbox__inner, .el-checkbox__input.is-indeterminate .el-checkbox__inner {
    background-color: hsl(43, 96%, 56%) !important;
    border-color: #fbbf24 !important;
  }
  .el-button--primary {
    border-color: #fbbf24 !important;
  }
  .el-button.el-button--default:hover:not(.is-disabled) {
    color: #606266;
    border-color: #2a2a2e !important;
    background-color: #2a2a2e !important;
  }
  #app .sidebar-container {
    -webkit-transition: width .28s;
    transition: width .28s;
    width: 250px !important;
    background-color: var(--menu-bg);
    height: 100%;
    position: fixed;
    font-size: 0;
    top: 50px;
    bottom: 0;
    left: 0;
    z-index: 1001;
    overflow: hidden;
    -webkit-box-shadow: 0 0 8px rgba(0, 0, 0, .1);
    box-shadow: 0 0 8px rgba(0, 0, 0, .1);
  }
  .el-table--border::after, .el-table--group::after {
    top: 0;
    right: 0;
    width: 1px;
    height: 100%;
    background-color: #2a2a2e !important;
  }
  .el-table::before {
    left: 0;
    bottom: 0;
    width: 100%;
    height: 1px;
    background-color: #2a2a2e !important;
  }
  .table-content[data-v-27b00672] .el-table__header thead>tr>th {
    border-bottom: 1px solid #2a2a2e !important;
  }
  .el-radio__input.is-checked .el-radio__inner {
    border-color: #fbbf24 !important;
    background: #fbbf24 !important;
  }
  .el-menu {
    border-right: solid 1px #e6e6e6;
    list-style: none;
    position: relative;
    margin: 0;
    padding-left: 0;
    background-color: #18181b !important;
  }
  .el-menu--vertical .nest-menu .el-submenu-sidebar>.el-submenu__title:hover, .el-menu--vertical .el-menu-item:hover {
    background-color: #2a2a2e !important;
  }
  .left-menu.el-menu .el-submenu-sidebar.el-submenu.is-opened {
    border-top: solid 1px #2a2a2e !important;
  }
  .el-loading-mask {
    position: absolute;
    z-index: 2000;
    background-color: #2a2a2e !important;
    margin: 0;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    -webkit-transition: opacity .3s;
    transition: opacity .3s;
  }
  .el-loading-spinner {
    top: 50%;
    margin-top: -21px;
    width: 100%;
    text-align: center;
    position: absolute;
    color: #fbbf24;
  }
  .switch-date[data-v-e545c94e] .switch {
    background-color: #000 !important;
}
</style>
