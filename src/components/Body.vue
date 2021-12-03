<template>
  <div class="heroBlock">
    <v-carousel cycle hide-delimiters>
      <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
        reverse-transition="fade-transition"
        transition="fade-transition"
      >
        <v-row class="title fill-height hidden-xs-only" align="center" justify="center">{{ item.title }}</v-row>
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
export default {
  name: "Body",
  data() {
    return {
      items: [
        {
          src: require("../assets/images/carousel_1.jpg"),
          title: "We are creative"
        },
        {
          src: require("../assets/images/carousel_2.jpg"),
          title: "We are hard worker"
        },
        {
          src: require("../assets/images/carousel_3.jpg"),
          title: "We are professional"
        }
      ]
    };
  }
};
</script>