<template>
    <div>
        <b-navbar toggleable="lg" type="dark" variant="info">
            <div class="container">
            <b-navbar-brand href="#">NavBar</b-navbar-brand>

            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>


            <!-- Right aligned nav items -->
            <b-navbar-nav class="ml-auto">
                <li class="nav-item"><a href="#" class="text-white">Hi</a></li>
                <li class="nav-item"><a href="#" class="text-white">Hi</a></li>
            </b-navbar-nav>

            </b-collapse>
            </div>
        </b-navbar>
</div>
</template>
<script>
export default {
    name: 'nav',
}
</script>

<style scoped>
.nav-item{
    padding: 0px 10px;
}
</style>