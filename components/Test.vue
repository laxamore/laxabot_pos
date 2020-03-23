<template>
    <div class="wrapper">
        <!-- Sidebar -->
        <b-nav vertical pills>
            <b-nav-item to="#" active>Dashboard</b-nav-item>
            <b-nav-item to="#">Services</b-nav-item>
            <b-nav-item to="#">Clients</b-nav-item>
            <b-nav-item to="#">Contact</b-nav-item>
        </b-nav>
        <!-- Page Content -->
        <div id="content">
            <!-- We'll fill this with dummy content -->
        </div>

    </div>
</template>

<script>
import '../assets/scss/style.scss'

export default {
    name: 'Test',
    props: {
        msg: String
    }
}
</script>