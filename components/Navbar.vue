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


      <v-menu
        top
        :close-on-content-click="closeOnContentClick"
      >
        <template v-slot:activator="{ on }">
          <v-btn
            small
            light
            v-on="on"
            class="menu-btn"
          >
            <v-icon>mdi-menu</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item
            v-for="(item, index) in items"
            nuxt-link
            :href="item.link"
            v-bind:key="item.icon"
          >
            <v-icon left small>{{ item.icon }}</v-icon>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>


      <v-btn class="send-request-big" light color="#F8EC48" link href="https://forms.gle/UKpj82JGUBMz9Kvd6" target="blank">
        Отправить заявку
      </v-btn>

      <template #extension>
        <v-btn class="send-request-small" light small color="#F8EC48" link href="https://forms.gle/UKpj82JGUBMz9Kvd6" target="blank">
         Отправить заявку
        </v-btn>
        <v-toolbar-items
          v-for="(item, index) in items"
          v-bind:key="item.icon"
        >
          <v-btn tile outlined text
          nuxt-link
          :href="item.link"
          >
            <v-icon left small>{{ item.icon }}</v-icon>
            {{ item.title }}
          </v-btn>
        </v-toolbar-items>
      </template>

    </v-app-bar>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: 'Положение', icon: 'mdi-file', link: '/rules' },
      { title: 'Контакты', icon: 'mdi-phone', link: '/contacts' },
    ],
    closeOnContentClick: true,
  }),
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
  @media (max-width: 499px) {
    .v-toolbar__items,
    .send-request-big {
      display: none !important;
    }
  }
  @media (max-width: 630px) {
    .v-toolbar__title small {
      display: none !important;
    }
  }
  @media (min-width: 500px) {
    .menu-btn,
    .send-request-small {
      display: none !important;
    }
  }
</style>
