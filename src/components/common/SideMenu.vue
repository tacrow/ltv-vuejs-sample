<template>
  <nav class="p-side-menu">
    <h2 class="p-nav-header">解析</h2>
    <ul class="p-nav-list"></router-link></li>
      <router-link tag="li" to="/" class="p-nav-list__item" exact><a>アクセス解析</a></router-link>
      <router-link tag="li" to="/send" class="p-nav-list__item"><a>送客元解析</a></router-link>
      <router-link tag="li" to="/search" class="p-nav-list__item"><a>複合検索解析</a></router-link>
      <router-link tag="li" to="/ip_log" class="p-nav-list__item"><a>利用者IPログ</a></router-link>
    </ul>
    <h2 class="p-nav-header">LTV解析</h2>
    <ul class="p-nav-list">
    </ul>
    <h2 class="p-nav-header">各種マスタ登録</h2>
    <ul id="nav-list2" class="p-nav-list">
      <router-link tag="li" to="/a" class="p-nav-list__item"><a>単価条件マスタ</a></router-link>
      <router-link tag="li" to="/b" class="p-nav-list__item"><a>ページ名称マスタ</a></router-link>
      <router-link tag="li" to="/c" class="p-nav-list__item"><a>複合検索名称マスタ</a></router-link>
      <router-link tag="li" to="/d" class="p-nav-list__item"><a>KWIDマスタ</a></router-link>
      <router-link tag="li" to="/e" class="p-nav-list__item"><a>LTV指標マスタ</a></router-link>
    </ul>
    <h2 class="p-nav-header">LTV実績アップロード</h2>
    <ul class="p-nav-list">
    </ul>
  </nav>
</template>

<style scoped>
.p-side-menu {
  float: left;
  width: 180px;
}
.p-nav-header {
  margin-bottom: 5px;
  border-bottom: 1px solid #eeeeee;
}
.p-nav-list {
  margin-bottom: 20px;
}
.p-nav-list__item {
  position: relative;
  margin-bottom: 5px;
  @mixin fs12;
  line-height: 1;
  &:last-child {
    margin-bottom: 0;
  }
  a {
    padding: 7px 0 6px 6px;
    color: #333333;
    transition: color .1s;
  }
  &::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 24px;
    background-color: #666666;
    opacity: 0;
    z-index: -1;
    transition: width .2s;
  }
  &:hover {
    transition: all .3s;
    a {
      color: #ffffff;
      transition: color .3s;
    }
    &::after {
      width: 100%;
      opacity: 1;
      transition: width .5s, opacity .5s;
    }
  }
  &.router-link-active {
    a { color: #ffffff; }
    &::after {
      width: 100%;
      opacity: 1;
    }
  }
}
</style>