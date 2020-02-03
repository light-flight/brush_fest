<template>
  <div>
    <v-footer
      dark
      padless
    >
      <v-card
        flat
        tile
        class="white--text text-center footer-card"
        color="#6B4791"
      >

        <v-card-text>
          <v-btn outlined class="mx-4 mb-3 white--text">
            <v-icon left link href="https://www.instagram.com/brush_fest/" target="_blank">mdi-instagram</v-icon>
            Instagram
          </v-btn>
          <v-btn class="mb-3" light color="#F8EC48" link href="https://forms.gle/UKpj82JGUBMz9Kvd6" target="blank">
            Отправить заявку
          </v-btn>
        </v-card-text>

        <v-btn
          v-for="(item, i) in items"
          :key="i"
          link
          :href="item.link"
          class="px-6"
          small
          text
        >
          <v-icon v-text="item.icon" left small></v-icon>
          {{ item.text }}
        </v-btn>

        <v-card-text class="white--text pt-0">
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>BRUSH</strong> Танцевальный фестиваль
        </v-card-text>
      </v-card>
    </v-footer>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: [
      { text: '8(903)798-41-02', icon: 'mdi-phone', link: 'tel:+79037984102' },
      { text: '8(495)571-21-58', icon: 'mdi-phone', link: 'tel:+74955712158' },
      { text: 'brush.festival@gmail.com', icon: 'mdi-email', link: 'mailto:brush.festival@gmail.com' },
    ],
  }),
}
</script>

<style lang="scss">
  .footer-card {
    width: 100%;
  }
  .contacts-links {
    display: inline-block;
  }
</style>
