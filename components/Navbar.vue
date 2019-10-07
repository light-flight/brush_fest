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
        <small v-if="$vuetify.breakpoint.smAndUp">Танцевальный фестиваль</small>
      </v-toolbar-title>


      <div class="flex-grow-1"></div>


      <v-menu
        top
        :close-on-content-click="closeOnContentClick"
        v-if="$vuetify.breakpoint.xsOnly"
      >
        <template v-slot:activator="{ on }">
          <v-btn
            small
            light
            v-on="on"
          >
            <v-icon>mdi-menu</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item
            v-for="(item, index) in items"
            nuxt-link
            :href="item.link"
          >
            <v-icon left small>{{ item.icon }}</v-icon>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>


      <v-btn v-else light color="#F8EC48" link href="https://forms.gle/UKpj82JGUBMz9Kvd6" target="blank">
        Отправить заявку
      </v-btn>


      <template #extension v-if="$vuetify.breakpoint.xsOnly">
        <v-btn light small color="#F8EC48" link href="https://forms.gle/UKpj82JGUBMz9Kvd6" target="blank">
         Отправить заявку
        </v-btn>
      </template>
      <template #extension v-else>
        <v-toolbar-items
          v-for="(item, index) in items"
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
</style>
