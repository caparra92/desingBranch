<template>
  <div class="w-full m-0 mb-0 pt-2 leading-tight">
    <h1 :class='"text-"+titleSize+"xl"'>{{ title | toUpper }}</h1>
    <h2 :class='"text-"+size+"xl pl-"+pl+" text-"+color'>{{ subtitle | toUpper }}</h2>
  </div>
</template>

<script>
export default {
    name: 'MainHeader',
    props: {
      title: {
        type: String,
        default: 'Social Media Post'
      },
      subtitle: {
        type: String,
        default: 'Business events'
      },
      color: {
        type: String,
        default: 'white'
      },
      size: {
        type: String,
        default: '2'
      },
      titleSize: {
        type: String,
        default: '3'
      },
      pl: {
        type: String,
        default: "0"
      }
    },
    filters: {
      toUpper(value) {
        return value.toUpperCase()
      }
    }
}
</script>

<style>

</style>