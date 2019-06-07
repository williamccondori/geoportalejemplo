<template lang="pug">
    section
        gnavbar
        .container-fluid
            .row
                .col-xs-24.col-sm-4.col-md-4.col-lg-4
                    .panel.panel-default
                        .panel-heading
                            h3.panel-title Capas
                        .panel-body Información de las capas
                .col-xs-24.col-sm-20.col-md-20.col-lg-20
                    gmap
</template>

<script>
import gnavbar from "~/components/geoportal/gnavbar.vue";
import gmap from "~/components/geoportal/gmap.vue";

export default {
  data() {
    return {
      message: "Hola Mundo!"
    };
  },
  components: {
    gnavbar,
    gmap
  }
};
</script>

<style lang="sass" scoped>

</style>