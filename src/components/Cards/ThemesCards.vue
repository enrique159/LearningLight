<template>
  <div>
    <v-row>
      <v-col cols="6">
        <div class="tarjeta">
          <div class="ilustracion">
            <img src="@/assets/books.svg" alt="Imagen" />
          </div>
          <span>Educación</span>
        </div>
      </v-col>
      <v-col cols="6">
        <div class="tarjeta">
          <div class="ilustracion">
            <img src="@/assets/working.svg" alt="Imagen" />
          </div>
          <span>Productividad</span>
        </div>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="6">
        <div class="tarjeta">
          <div class="ilustracion">
            <img src="@/assets/smartphone.svg" alt="Imagen" />
          </div>
          <span>Tecnología</span>
        </div>
      </v-col>
      <v-col cols="6">
        <div class="tarjeta">
          <div class="ilustracion">
            <img src="@/assets/school.svg" alt="Imagen" />
          </div>
          <span>Universidad</span>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.tarjeta {
  border-radius: 12px;
  background-color: #eff0ff;
  background-position: center;
  background-size: 100px;
  padding: 24px 18px 12px;
  text-align: center;
  height: 128px;

  span {
    font-size: 14px;
    font-weight: 500;
    color: rgb(64, 42, 101);
  }

  .ilustracion {
    img {
      height: 48px;
      margin-bottom: 16px;
    }
  }
}
</style>