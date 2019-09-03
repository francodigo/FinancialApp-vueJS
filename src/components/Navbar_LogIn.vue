<template>
    <b-navbar toggleable="lg" type="light" variant="light" class="shadow">
        <b-container>
            <b-navbar-brand href="#">Financial</b-navbar-brand>

            <b-navbar-toggle target="nav-collapse" class="border-0"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item href="#">Ultimos Movimientos</b-nav-item>
                    <b-nav-item href="#">Historicos</b-nav-item>
                    <b-nav-item href="#">Ingresos</b-nav-item>
                    <b-nav-item href="#">Egresos</b-nav-item>
                </b-navbar-nav>

                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto">

                    <b-nav-item-dropdown right>
                        <!-- Using 'button-content' slot -->
                        <template slot="button-content">
                            <img class="img-user"> User Name  
                        </template>
                        <b-dropdown-item href="#">Profile</b-dropdown-item>
                        <b-dropdown-item href="#">Sign Out</b-dropdown-item>
                    </b-nav-item-dropdown>
                </b-navbar-nav>

            </b-collapse>
        </b-container>
    </b-navbar>
</template>



<script>
    export default {

    }    
</script>


<style>
.img-user {
    width: 32px;
    height: 32px;
    position: absolute;
    left: -28px;
    bottom: 5px;
    border-radius: 50%;
    background-image: url("https:\/\/randomuser.me\/api\/portraits\/women\/20.jpg");
}

/* Medium devices (tablets, less than 992px) */
@media (max-width: 991.98px) { 
    .img-user{
        display: none;
    }
 }

</style>