<template>
  <v-container class="homeworkStats">
    <v-row class="espacios">
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
      <v-col
        class="tarea"
        cols="12"
        v-for="tarea in tareas"
        :key="tarea.asignatura"
      >
        <span>{{ tarea.asignatura }}</span>
        <v-progress-linear
          id="ProgressTarea"
          color="#525ADF"
          rounded
          :value="tarea.porcentaje"
        ></v-progress-linear>
        <v-row justify="space-between">
          <v-col cols="9">
            <span>{{ tarea.modulos }}</span>
          </v-col>
          <v-col cols="2">
            <span>{{ tarea.porcentaje }}% </span>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      tareas: [
        {
          asignatura: "Álgebra Lineal",
          porcentaje: 80,
          modulos: "5/8",
        },
        {
          asignatura: "Bases de Tipografía",
          porcentaje: 50,
          modulos: "4/8",
        },
        {
          asignatura: "Taller de Diseño",
          porcentaje: 50,
          modulos: "4/8",
        },
      ],
    };
  },
};
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

  .espacios{
    padding: 0px 8px;
  }

  .opcion {
    margin-bottom: 12px;
  }

  .tarea {
    padding: 8px 24px;

    span {
      font-size: 14px;
    }

    #ProgressTarea {
      margin-top: 12px;
    }
  }
}
</style>