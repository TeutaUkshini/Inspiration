<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/img13.jpg">
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
          <v-col>
            <v-container>
              <div class="headline">About Us</div>
            </v-container>
          </v-col>
        </v-row>
      </v-img>
    </div>
    <div class="block">
      <v-container>
        <p> Design and web design trends are always on the move. Creative folks from all around the world keep coming up with mind-blowing website layouts, bringing to life their best and most original ideas. So do the wedding photographers from the Flothemes community! No wonder, the new Flex builder allows them to easily materialize any concept or vision that they’ve had boiling in their mind for a while now, but couldn’t quite verbalize.</p>
      </v-container>
    </div>
    <div class="block">
      <v-container>
        <h2 class="text-center">Our Teams</h2>
        <v-row>
          <v-col v-for="item in items" :key="item.id" class="d-flex child-flex" cols="12" sm="4">
            <v-card flat tile class="mx-auto">
              <v-img :src="item.src" aspect-ratio="1" class="grey lighten-2"></v-img>
              <v-card-text class="text--primary text-center">
                <div class="title">{{ item.name }}</div>
                <p>{{ item.title }}</p>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </v-content>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      items: [
        {
          id: 1,
          src: require("../assets/images/team1.jpg"),
          name: 'Asheley Smith',
          title: 'Director'
        },
        {
          id: 2,
          src: require("../assets/images/team2.jpg"),
          name: 'Roy Perry',
          title: 'Photographer'
        },
        {
          id: 3,
          src: require("../assets/images/team3.png"),
          name: 'Lisa White',
          title: 'Freelancer'
        },
        {
          id: 4,
          src: require("../assets/images/team4.jpg"),
          name: 'Raul Maneksh',
          title: 'Photographer'
        },
        {
          id: 5,
          src: require("../assets/images/team5.jpg"),
          name: 'Noah Liam',
          title: 'Intern'
        },
        {
          id: 6,
          src: require("../assets/images/team6.jpg"),
          name: ' Amelia Campbell',
          title: 'Intern'
        }

      ]
    };
  }
};
</script>