<template>
    <!-- spacer -->
    <v-flex md1 lg2 />
    <v-flex md10 lg8>
      <!-- section title -->
      <v-flex xs12 mb-2 class="section-title">
        <a>함께하는 파트너</a>
      </v-flex>
      <!-- section link -->
      <v-flex xs12 mb-4 class="section-link">
        <a>함께하는 파트너</a>
      </v-flex>
      <slot />
    </v-flex>
    <!-- spacer -->
    <v-flex md1 lg2 />
</template>

<script>
      
export default {
  components: {},
  props: {
    paddingTop: {
      type: String,
      default: '46px',
    },
    paddingBottom: {
      type: String,
      default: '48px',
    },
    backgroundColor: {
      type: String,
      default: '#ffffff',
    },
  },
  computed: {
    containerStyle() {
      return {
        'padding-top': this.paddingTop,
        'padding-bottom': this.paddingBottom,
        'background-color': this.backgroundColor,
      };
    },
  },
};
</script>

<style lang="scss" scoped>
.layout-mobile {
  .section-link {
    margin-top: 0px;
    margin-bottom: 40px;
    text-align: center;
  }
}
</style>
