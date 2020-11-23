<template>
  <div class="contenedor">
    <Optionbar />
  </div>
</template>

<script>
import Optionbar from "./ContentHome/OptionBar";
export default {
  components: {
    Optionbar,
  },
};
</script>

<style lang="scss" scoped>
.contenedor {
  padding-left: 256px;
  margin-top: 62px;
  width: 100%;
  float: left;
}
</style>