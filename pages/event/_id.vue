<template>
  <div>
    <h1>Events #{{ id }}</h1>
  </div>
</template>

<script>
export default {
  computed: {
    id() {
      return this.$route.params.id
    },
  },
  head() {
    return {
      title: 'Event ID #' + this.id,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'what you need to know about event #' + this.id,
        },
      ],
    }
  },
}
</script>
