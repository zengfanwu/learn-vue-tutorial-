<template>
    <div id="wrapper">
        <nav class="navbar navbar-default">
            <div class="contanier">
                <a href="#" class="navbar-brand">
                    <i class="glyphicon glyphicon-time">计划板</i>
                </a>
                <ul class="nav navbar-nav">
                    <li>
                        <router-link to="/home">首页</router-link>
                    </li>
                    <li>
                        <router-link to="/time-entries">计划列表</router-link>
                    </li>
                </ul>
            </div>
        </nav>
        <div class="contanier">
            <div class="col-sm-3">
                <sidebar></sidebar>
            </div>
            <div class="col-sm-9">
                <router-view></router-view>
            </div>
        </div>
    </div>
</template>

<script>
    import Sidebar from './components/Sidebar.vue'

    export default {
        components: {
            'sidebar': Sidebar
        }
    }
</script>

<style lang="css">
</style>
