<template>
  <div class="wrapper-content">
    <slot />
  </div>
</template>

<script>
export default {
  name: 'PageContent'
}
</script>

<style scoped>
  .wrapper-content {
    padding: 24px 24px 22px;
    background-color: #141416;
  }

  .wrapper-content >>> .el-button--primary {
    background-color: #27a12f;
    border-color: none;
  }

  .wrapper-content >>>  .el-input__inner {
    background-color: #111113;
    border: 1px solid #2a2a2e;
    color: white;
  }

  .wrapper-content >>> .el-button--primary.is-plain {
    color: white;
    border-color: none;
  }

  .wrapper-content >>> .el-button--default {
    background-color: #3c3f43;
    border: 0px;
    border-color: none;
    color: white;
  }

  .wrapper-content >>> .el-alert {
    margin-bottom: 15px;
  }

  .wrapper-content >>> .el-table tr {
    background-color: #18181b;
  }

  .wrapper-content >>> .table-content {
    border: 1px solid #2a2a2e;
  }

  .page-alert >>> .el-alert {
    margin-bottom: 20px;
  }

  .wrapper-content  >>> .el-pagination.is-background .btn-prev {
    background-color: #18181b;
    border: 1px solid #2a2a2e;
  }

  .wrapper-content  >>> .el-pagination.is-background .btn-next {
    background-color: #18181b;
    border: 1px solid #2a2a2e;
  }

  .wrapper-content >>> .el-pagination.is-background .el-pager li:not(.disabled).active{
    background-color: #18181b;
    border: 1px solid #fbbf24;
    color: #fbbf24;
  }

  .wrapper-content >>> .el-table--border, .el-table--group {
    border: 1px solid #2a2a2e;
  }

  .wrapper-content >>> .el-table__header-wrapper {
    border: 0px solid;
  }

  .wrapper-content >>> .el-table__empty-block {
    background-color:#18181b;
  }

  .wrapper-content >>> .el-tabs__nav-wrap {
    background-color: #111113;
    color: white;
  }

  .wrapper-content >>> .page-submenu[data-v-c173972c] .el-tabs__header {
    background-color: #111113;
    color: white;
  }

  .wrapper-content >>> .el-tabs__nav-prev {
    background-color: #111113;
    color: #fbbf24;
  }

  .wrapper-content >>> .el-tabs__nav-next {
    background-color: #111113;
    color: #fbbf24;
  }

  .wrapper-content >>> .el-tabs__item {
    background-color: #111113;
    color: #fff;
  }

  .wrapper-content >>> .el-card {
    background-color: #111113;
    color: #fff;
  }

  .wrapper-content >>> .el-dropdown-menu .el-popper {
    background-color: #111113;
    color: #fff;
  }

  .page-alert >>> .el-alert {
    margin-bottom: 20px;
  }
</style>
