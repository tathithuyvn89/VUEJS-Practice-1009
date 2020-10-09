<template>
  <el-row>
      
        <el-col :span="20" class="navbar__menu-box">
            <ul class="el-menu el-menu--horizontal navbar__menu">
                <li class="el-menu-item">菜单1</li>
                <li class="el-menu-item">菜单2</li>
                <li class="el-menu-item">
                    <el-dropdown trigger="click" v-on:command="handleNavDropdownCommand">
                        <span class="el-dropdown-link">13999999999 <i class="el-icon-caret-bottom el-icon--right"></i></span>
                        <el-dropdown-menu slot="dropdown" class="navbar__dropdown-menu">
                            <el-dropdown-item><router-link to="/user/recharge">账户充值</router-link></el-dropdown-item>
                            <el-dropdown-item><router-link to="/user/account">账户信息</router-link></el-dropdown-item>
                            <el-dropdown-item command="logout" divided>退出</el-dropdown-item>
                        </el-dropdown-menu>
                    </el-dropdown>
                </li>
                <li class="el-menu-item" >Login</li>
                <li class="el-menu-item">Logout</li>
            </ul>
            <p class="navbar__title"><a href="https://github.com/appbone/element-ui-admin">element-ui-admin</a></p>
        </el-col>
    </el-row>
</template>

<script>
export default {
  name: 'Header'

}
</script>

<style>

</style>