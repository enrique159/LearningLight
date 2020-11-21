<template>
  <div>
    <Appbar/>
    <Drawmenu/>
    <Optionbar/>
  </div>
</template>

<script>
import Appbar from './components/Appbar'
import Drawmenu from './components/Drawmenu'
import Optionbar from './components/Optionbar'

export default {
  name: "App",
  data: () => ({
    //
  }),
  components: {
    Appbar,
    Drawmenu,
    Optionbar
  },
};
</script>

<style lang="scss">
  
body{
  font-family: 'Montserrat', Tahoma, Geneva, Verdana, sans-serif;
}

</style>
