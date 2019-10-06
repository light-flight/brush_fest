<template>
  <div class="container">
    <h1>Предстоящие события</h1>
    <v-sheet class="event" elevation='5'>
      <img src="poster.jpg" alt="" class="poster">
      <div class="info">
        <ul class="info-list">
          <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet dolore unde quisquam fugiat magnam molestiae quam nihil officia, dignissimos consequatur debitis quis veritatis dolorum ab necessitatibus dolores odit culpa esse!</li>
          <li></li>
          <li></li>
          <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Officiis, corporis adipisci qui sed dicta et sint. Architecto quisquam voluptates fugiat modi id eaque vero explicabo, atque, expedita hic nesciunt reiciendis!</li>
          <li></li>
        </ul>
      </div>
      <div class="map">
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2242.534533899662!2d37.67041031552495!3d55.80131999571701!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46b535be0f476dd1%3A0x79e01f70b9c2483f!2zNC3QuSDQm9GD0YfQtdCy0L7QuSDQv9GA0L7RgdC10LosIDQsINCc0L7RgdC60LLQsCwgMTA3MDE0!5e0!3m2!1sru!2sru!4v1570398421926!5m2!1sru!2sru" frameborder="0" style="border:0;" allowfullscreen=""></iframe>
      </div>
    </v-sheet>
  </div>
</template>

<script>
  export default {
  }
</script>

<style lang="scss" scoped>
  h1 {
    margin-top: .75em;
    margin-bottom: .5em;
  }
  .poster {
    display: block;
    width: 100%;
  }
  .map {
    iframe {
      width: 100%;
      min-height: 400px;
    }
  }
</style>
