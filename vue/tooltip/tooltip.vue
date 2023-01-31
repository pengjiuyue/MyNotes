<template>
  <v-tooltip bottom>
    <template v-slot:activator="{ on, attrs }">
      <div v-bind="attrs" v-on="on"></div>
    </template>
    <span>Not supported on V2 devices.</span>
  </v-tooltip>
</template>

<script>
export default {
  data() {
    return {};
  },
  computed: {},

  methods: {},
};
</script>

<style scoped lang="scss"></style>
