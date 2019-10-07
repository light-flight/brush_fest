<template>
  <div class="container">
    <h1>Предстоящие события</h1>
    <v-sheet class="event" elevation='5' color="white">
      <div class="image">
        <img src="poster.jpg" alt="" class="poster">
      </div>
      <div class="info-block">
        <div class="info-list">
          <v-list disabled>
            <v-list-item-group>
              <v-list-item
                v-for="(item, i) in items"
                :key="i"
              >
                <v-list-item-icon>
                  <v-icon v-text="item.icon"></v-icon>
                </v-list-item-icon>
                <v-list-item-content>
                  <v-list-item-title v-text="item.text"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </div>
        <iframe class="info-map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2242.534533899662!2d37.67041031552495!3d55.80131999571701!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46b535be0f476dd1%3A0x79e01f70b9c2483f!2zNC3QuSDQm9GD0YfQtdCy0L7QuSDQv9GA0L7RgdC10LosIDQsINCc0L7RgdC60LLQsCwgMTA3MDE0!5e0!3m2!1sru!2sru!4v1570398421926!5m2!1sru!2sru" frameborder="0" style="border:0;" allowfullscreen=""></iframe>
      </div>
    </v-sheet>
  </div>
</template>

<script>
  export default {
    data: () => ({
      items: [
        { text: '20 октября 2019г.', icon: 'mdi-calendar' },
        { text: 'Москва, 4-й Лучевой просек, 4', icon: 'mdi-city' },
        { text: 'kopytnikoff@yandex.ru', icon: 'mdi-email' },
        { text: '8(903)798-41-02', icon: 'mdi-phone' },
      ],
    }),
  }
</script>

<style lang="scss" scoped>
  .container {
    max-width: 1000px;
  }
  h1 {
    margin-top: .75em;
    margin-bottom: .5em;
  }
  .poster {
    display: block;
    width: 100%;
  }
  .info-block {
    width: 100%;
  }
  .info-map {
    display: block;
    width: 100%;
    min-height: 200px;
  }
  @media (min-width: 500px) {
    .event {
      display: -webkit-flex;
      display: -ms-flex;
      display: flex;
      width: 100%;
      margin-bottom: 3em;
    }
    .image {
      flex: 0 0 40%;
    }
    .info-block {
      display: -webkit-flex;
      display: -ms-flex;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      .v-list {
        padding: 0;
      }
      .info-map {
        flex: 1 1 auto;
      }
    }
  }
</style>
