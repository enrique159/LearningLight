<template>
  <div class="contenedor">
    <Optionbar />
    <Articles />
    <VideoAndTeachers />
  </div>
</template>

<script>
import Optionbar from "./ContentHome/OptionBar";
import Articles from "./ContentHome/Articles";
import VideoAndTeachers from "./ContentHome/VideoAndTeachers"

export default {
  components: {
    Optionbar,
    Articles,
    VideoAndTeachers
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