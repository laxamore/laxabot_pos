<template>
    <div class="wrapper">
        <!-- Page Content -->
        <div class="content">
            <!-- We'll fill this with dummy content -->
            <h1>
                {{msg}}
            </h1>
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