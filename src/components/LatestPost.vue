<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">Latest Post</h2>
      <v-row>
        <v-col v-for="item in items" :key="item.id" cols="12" md="4">
          <v-card outlined class="mx-auto">
            <v-img
              class="white--text align-end"
              height="200px"
              :src="item.src"
            >
              <v-card-title>{{ item.title }}</v-card-title>
            </v-img>
            <v-card-subtitle class="pb-0">{{ item.subtitle }}</v-card-subtitle>
            <v-card-text class="text--primary">
              <div>{{ item.description }}</div>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "LatestPost",
  data: () => ({
    show: false,
    items: [
      {
        id: 1,
        title: "Top western road trips",
        subtitle: "1,000 miles of wonder",
        description: "We're working to prevent them everywhere. But it is urgently required to become accustomed. This website is not as bad as it is. While it may sound exciting from being roasted, it may have deterred the camera from using it to tell stories about it at some point.",
        src: require("../assets/images/img10.jpg")
      },
      {
        id: 2,
        title: "Christmas tales to read",
        subtitle: "2,000 miles of wonder",
        description: "We have to become accustomed to the sea, and we all agree that Plato is, at all times, a danger to himself. The website is an elegant definition of a young man who, in his opinion, did something right. The camera from using it to tell stories about it at some point.",
        src: require("../assets/images/img11.jpg")
      },
      {
        id: 3,
        title: "20 movies not to miss in 2021",
        subtitle: "3,000 miles of wonder",
        description: "Some of my whites will be written to him, due to the collar and pro, that they will be written no. They think you're an organized amalgamation of people. Young man, you are pursuing violence against him. You can't be checked either. The camera from using it to tell stories about it ",
        src: require("../assets/images/img12.jpg")
      }
    ]
  })
};
</script>