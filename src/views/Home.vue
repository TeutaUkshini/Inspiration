<template>
  <v-content>
    <Body />
    <Gallery />
    <LatestPost />
  </v-content>
</template>

<script>
import Body from "../components/Body";
import Gallery from "../components/Gallery";
import LatestPost from "../components/LatestPost";

export default {
  name: "Home",

  components: {
    Body,
    Gallery,
    LatestPost,
  }
};
</script>