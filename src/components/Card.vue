<template>
  <div :class='"w-full shadow-xs "+gradient'>
      <slot name="cardHeader"></slot>
      <slot name="cardContent"></slot>
  </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
      gradient: {
        type: String,
        default: 'by'
      }
    }
}
</script>

<style>
.by {
  background: linear-gradient(180deg, #004a89 80%, #fdbe42 20%);
}
.wb {
  background: linear-gradient(160deg, #fff 45%, #004a89 40%);
}
.shape {
  background-image: url('../assets/img/twogirls.png');
  background-size: cover;
  background-repeat: no-repeat;
}
.shape2 {
  background-image: url('../assets/img/2girls.png');
  background-size: cover;
  background-repeat: no-repeat;
}

</style>