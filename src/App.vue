<template>
  <div>
    <Appbar/>
    <Drawmenu/>
    <ContentHome/>
  </div>
</template>

<script>
import Appbar from './components/Appbar'
import Drawmenu from './components/Drawmenu'
import ContentHome from './components/ContentHome'

export default {
  name: "App",
  data: () => ({
    //
  }),
  components: {
    Appbar,
    Drawmenu,
    ContentHome
  },
};
</script>

<style lang="scss">
  
body{
  font-family: 'Montserrat', Tahoma, Geneva, Verdana, sans-serif;
}

</style>
