<template>
  <div>
    <v-app-bar
      color="#6B4791"
      dark
      extended
      class="main-app-bar"
    >
      <img src="logo.png" class="logo"/>
      <v-toolbar-title>
        BRUSH
        <small>Танцевальный фестиваль</small>
      </v-toolbar-title>
      <div class="flex-grow-1"></div>
      <v-btn light color="#F8EC48" link href="https://forms.gle/UKpj82JGUBMz9Kvd6" target="blank">
        Отправить заявку
      </v-btn>

      <template #extension>
        <v-toolbar-items>
          <v-btn tile outlined text>
            <v-icon left small>mdi-file</v-icon>
            Положение
          </v-btn>
          <v-btn tile outlined text>
            <v-icon left small>mdi-phone</v-icon>
            Контакты
          </v-btn>
          <!-- <v-btn tile outlined text>
            <v-icon left small>mdi-image</v-icon>
            Фотогалерея
          </v-btn> -->
        </v-toolbar-items>
      </template>
    </v-app-bar>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="scss">
  img.logo {
    width: 110px;
    position: absolute;
    left: 4px;
    top: 0;
  }
  .main-app-bar {
    .v-toolbar__content,
    .v-toolbar__extension {
      padding-left: 116px;
    }
  }
</style>
