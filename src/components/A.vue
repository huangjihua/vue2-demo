<template lang="html">
  <div class="a">
       <input type="date" v-model="myData" placeholder="Date" />
       <button @click="save()">保存</button>
  </div>
</template>

<script>
export default {
  data  () {
    return {
      myData: 'myData'
    };
  },
  computed: {},
  ready () {},
  attached  () {},
  methods: {
    save () {
      let value = this.myData
      this.update(value)
    }
  },
  vuex: {
    actions: {
      update: function ({dispatch}, value) {
        dispatch('UPDATE', value)
      }
    }
  },
  components: {}
};
</script>

<style lang="css">
  .a {
     border: solid 1px rgb(238, 64, 237);
     padding: 10px;
  }
</style>
