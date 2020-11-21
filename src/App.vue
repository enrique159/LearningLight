<template>
  <div>
    <Appbar/>
    <Drawmenu/>
  </div>
</template>

<script>
import Appbar from './components/Appbar'
import Drawmenu from './components/Drawmenu'

export default {
  name: "App",
  data: () => ({
    //
  }),
  components: {
    Appbar,
    Drawmenu
  },
};
</script>

<style lang="scss">
  
body{
  font-family: 'Montserrat', Tahoma, Geneva, Verdana, sans-serif;
}

</style>
