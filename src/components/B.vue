<template lang="html">
  <div class="b">
     <p>{{myData}}</p>
  </div>
</template>

<script>
export default {
  data  () {
    return {
    };
  },
  computed: {},
  ready () {},
  attached  () {},
  methods: {},
  vuex: {
    getters: {
      myData: function (state) {
        return state.myData
      }
    }
  },
  components: {}
};
</script>

<style lang="css">
.b{ border: solid 1px rgb(38, 17, 166); }
</style>
