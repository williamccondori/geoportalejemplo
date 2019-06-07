<template lang="pug">
     nav.navbar.navbar-inverse.navbar-static-top(role='navigation')
        .container-fluid
            .navbar-header
                button.navbar-toggle(
                    type='button', 
                    data-toggle='collapse', 
                    data-target='.veox-menu')
                    span.icon-bar
                    span.icon-bar
                    span.icon-bar
                a.navbar-brand(href='') UNAT
            div.collapse.navbar-collapse.veox-menu
                ul.nav.navbar-nav
                    li
                        a(href='') Inicio
                    li
                        a(href='') Reportar
</template>

<script>
export default {
};
</script>

<style scoped>
</style>