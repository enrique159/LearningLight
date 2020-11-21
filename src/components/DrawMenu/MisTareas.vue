<template>
  <v-container class="homeworkStats">
    <v-row>
      <v-col class="opcion" cols="12">
        <v-btn class="opcionbtn" depressed color="#FFFFFF">
          <v-row align="center">
            <v-icon medium color="#525ADF"> mdi-book </v-icon>
            <span id="mistareas">Mis Tareas</span>
            <v-icon id="flechaderecha" medium color="#525ADF">
              mdi-arrow-right
            </v-icon>
          </v-row>
        </v-btn>
      </v-col>
      <v-col class="tarea" cols="12">
        <span>Álgebra Lineal</span>
        <v-progress-linear
          id="ProgressTarea"
          color="#525ADF"
          rounded
          value="80"
        ></v-progress-linear>
        <v-row justify="space-between">
          <v-col cols="9">
            <span>5/8</span>
          </v-col>
          <v-col cols="2">
            <span>80%</span>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.homeworkStats {
  #mistareas {
    color: #252525;
  }

  #flechaderecha {
    position: absolute;
    right: 0px;
  }

  .tarea{
    padding: 24px;

    #ProgressTarea{
      margin-top: 12px;
    }
  }
}
</style>