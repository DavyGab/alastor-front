<template>
  <div id="main-wrapper">
        <!-- header header  -->
        <TopBar/>
        <!-- End header header -->


        <!-- Left Sidebar  -->
        <LeftMenu/>
        <!-- End Left Sidebar  -->


        <!-- Page wrapper  -->
        <div class="page-wrapper">
            <!-- Bread crumb -->
            <Breadcrumb/>
            <!-- End Bread crumb -->
            <!-- Container fluid  -->

            <div class="container-fluid">
                <div class="row">
                    <div class="col-6">
                        <TableDeadline/>
                    </div>
                </div>
            </div>
            <!-- End Container fluid  -->
            <!-- footer -->
            <footer class="footer">© 2018 All rights reserved. Created by Davy</footer>
            <!-- End footer -->
        </div>
        <!-- End Page wrapper  -->
    </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Breadcrumb from './components/Navigation/Breadcrumb.vue'
import LeftMenu from './components/Navigation/LeftMenu.vue'
import TopBar from './components/Navigation/TopBar.vue'

import TableDeadline from './components/TableDeadline.vue'

export default {
	components: {
		Breadcrumb,
        LeftMenu,
        TopBar,
        TableDeadline
	}
}
</script>

<style>
</style>
