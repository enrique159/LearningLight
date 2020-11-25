<template>
  <v-row>
    <v-col cols="7">
      <div class="tarjeta"> 
        <div class="ilustracion">
          <img src="@/assets/Article1.svg" alt="Imagen" />
        </div>
        <h2>Principios del <br />diseño inclusivo</h2>
        <div class="tiempo">
          <v-icon small color="#614e81"> mdi-clock </v-icon>
          <span class="minutos">5 min</span>
        </div>
        <div class="profesor">
          <img
            src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQN8Hy0mTqlUq7se9R-Z6R8PKSwt4CVEdEIsQ&usqp=CAU"
            class="perfil"
            alt=""
          />
          <div class="datosProfesor">
            <h6>Alfredo Adame</h6>
            <span>Feb 11</span>
          </div>
        </div>
      </div>
    </v-col>
    <v-col cols="5">
      <div class="tarjeta">
        <div class="ilustracionSmall">
          <img src="@/assets/Article2.svg" alt="Imagen" />
        </div>
        <h2>Tendencias de <br />diseño 2021</h2>
        <div class="tiempo">
          <v-icon small color="#614e81"> mdi-clock </v-icon>
          <span class="minutos">1 min</span>
        </div>
        <div class="profesor">
          <img
            src="https://deythere.com/wp-content/uploads/2019/10/perfection-in-profile-royalty-free-image-1069713934-1555616257.jpg"
            class="perfil"
            alt=""
          />
          <div class="datosProfesor">
            <h6>Christine Sanchez</h6>
            <span>Ene 12</span>
          </div>
        </div>
      </div>
    </v-col>
  </v-row>
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
  position: relative;
  padding: 21px;
  height: 278px;

  h2 {
    font-weight: 400;
    font-size: 21px;
    color: rgb(64, 42, 101);
    margin-bottom: 32px;
  }

  .tiempo {
    padding: 4px 4px 6px 6px;
    background-color: #e4e5f5;
    border-radius: 8px;
    color: #614e81;
    width: fit-content;
    margin-bottom: 78px;
    .minutos {
      font-size: 14px;
      font-weight: 600;
      padding: 0px 4px;
    }
  }

  .profesor {
    .perfil {
      height: 48px;
      border-radius: 12px;
    }
    .datosProfesor {
      padding: 5px 8px;
      display: inline-block;
      position: absolute;
      h6 {
        font-size: 14px;
        font-weight: 500;
        color: rgb(64, 42, 101);
      }
      span {
        font-size: 12px;
        color: #614e81;
      }
    }
  }

  .ilustracion {
    position: absolute;
    top: 48px;
    right: 20px;
    img {
      height: 148px;
    }
  }
  .ilustracionSmall {
    position: absolute;
    top: 78px;
    right: 20px;
    img {
      height: 98px;
    }
  }
}
</style>