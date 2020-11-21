<template>
  <div class="topnav">
    <div class="logo acomodo">
      <button>
        <v-container fluid>
          <v-row>
            <img src="@/assets/logo.svg" alt="" />
            <h4>LearningLight</h4>
          </v-row>
        </v-container>
      </button>
    </div>
    <div class="searchbar acomodo">
      <v-row class="buscador">
        <v-icon id="searchicon" medium color="#9498C6"> mdi-magnify </v-icon>
        <input type="text" name="search" placeholder="Buscar..." />
      </v-row>
    </div>
    <div class="user acomodo">
      <v-row>
        <v-btn class="btnbell" color="#FFFFFF" depressed fab small>
          <v-icon id="searchicon" medium color="#252525"> mdi-bell </v-icon>
        </v-btn>
        <img
          src="@/assets/profile_picture.jpg"
          alt="Profile"
        />
        <span>David Fargan</span>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.topnav {
  background-color: rgb(255, 255, 255);
  border-bottom: 2px solid rgb(239, 240, 255);
  position: fixed;
  z-index: 10;
  width: 100%;

  .acomodo {
    display: inline-block;
  }

  .logo {
    border-right: 2px solid rgb(239, 240, 255);
    width: 256px;
    padding: 8px 48px 8px 32px;

    button {
      img {
        height: 21px;
        margin-right: 8px;
      }
      h4 {
        font-size: 19px;
        font-weight: 500;
        color: #252525;
      }
      &:hover {
        opacity: 0.8;
      }
      &:focus {
        outline: none;
      }
    }
  }

  .searchbar {
    width: 50%;
    max-width: 50vw;
    padding: 12px 48px 8px 48px;
    position: fixed;

    #searchicon {
      padding-right: 12px;
    }

    .buscador {
      font-size: 16px;
      line-height: 1.2;
      color: #9498c6;

      display: block;
      background: #eff0ff;
      border-radius: 6px;
      padding: 8px 18px;

      input {
        color: #5a5d7e;
        &:focus {
          border-style: none;
          outline: none;
        }
      }
      ::placeholder {
        /* Chrome, Firefox, Opera, Safari 10.1+ */
        color: #9498c6;
        opacity: 0.8; /* Firefox */
      }
    }
  }

  .user {
    padding: 8px 48px 8px 48px;
    float: right;
    vertical-align: middle;
    text-align: center;

    .btnbell {
      margin: 4px;
      margin-right: 24px;
    }

    img {
      margin-top: 3px;
      height: 42px;
      background-position: center; /* Center the image */
      background-repeat: no-repeat; /* Do not repeat the image */
      background-size: cover;
      border-radius: 24px;
    }

    span {
      margin-top: 14px;
      margin-left: 12px;
      text-align: center;
      font-weight: 500;
    }
  }
}
</style>