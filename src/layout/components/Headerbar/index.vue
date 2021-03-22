<template>
<div>
  <div class="headerbar">
    <div class="brandarea"><img class="logo-image" src="//www.baidu.com/img/flexible/logo/pc/result@2.png" alt="到百度首页" title="到百度首页"></div>
    <div class="menuarea">
        <ul role="menubar" class="el-menu-demo el-menu--horizontal el-menu">
            <li role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
                <a href="#/dashboard" class="">首页</a>
            </li>
            <li role="menuitem" aria-haspopup="true" class="el-submenu" tabindex="0">
                <div class="el-submenu__title" style="border-bottom-color: transparent;"><span>货源管理</span></div>
            </li>
            <li role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
                <a href="#/form/index" class="router-link-exact-active router-link-active">车辆预约</a>
            </li>
            <li role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
                <a href="#/form/index" class="router-link-exact-active router-link-active">运单管理</a>
            </li>
                        <li role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
                <a href="#/form/index" class="router-link-exact-active router-link-active">财务管理</a>
            </li>
        </ul>
    </div>
    <div class="endarea">
        <div>
            <span>你好，可用余额:</span> <span>199999</span>
        </div>
        <el-dropdown class="avatar-container" trigger="click">
        <div class="avatar-wrapper">
            <span>大宗智联</span>
            <i class="el-icon-caret-bottom" />
        </div>
            <el-dropdown-menu slot="dropdown" class="user-dropdown">
            <router-link to="/">
                <el-dropdown-item>
                个人信息
                </el-dropdown-item>
            </router-link>
            <router-link to="/">
                <el-dropdown-item>
                账号信息
                </el-dropdown-item>
            </router-link>
            <router-link to="/">
                <el-dropdown-item>
                修改密码
                </el-dropdown-item>
            </router-link>
            </el-dropdown-menu>
        </el-dropdown>
        <div>
            <a @click.native="logout"> 退出</a>
        </div>
    </div>
  </div>
  <div class="secondbar">
      <div class="brandarea"></div>
      <div class="menuarea">
        <ul role="menubar" class="el-menu-demo el-menu--horizontal el-menu">
            <li role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
                <a href="#/dashboard" class="">首页</a>
            </li>
            <li role="menuitem" aria-haspopup="true" class="el-submenu" tabindex="0">
                <div class="el-submenu__title" style="border-bottom-color: transparent;"><span>Example</span></div>
            </li>
            <li role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
                <a href="#/form/index" class="router-link-exact-active router-link-active">test</a>
            </li>
        </ul>
      </div>
  </div>
</div>
</template>

<script>

export default {
  components: {},
  computed: {

  }
}
</script>
