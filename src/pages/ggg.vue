<template lang="jade">
div
  h1 {{msg}}
  comp-b
  comp-a
</template>

<script>
import compA from '../components/a.vue'
import compB from '../components/b.vue'
export default {
  data () {
    return {
      msg: 'support!'
    }
  },
  components: {
    'comp-a': compA,
    'comp-b': compB
  },
  ready: function () {
    console.log("ggg");
    this.$dispatch('_locationchange');
  }
}
</script>
