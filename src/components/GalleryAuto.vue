<template>
  <v-container
    grid-list-lg
  >
    <v-layout row wrap>
      <v-flex
        xs12
        sm6
        v-for="(card, index) in cards"
        v-bind="{ [`lg${card.flex}`]: true }"
        :key="card.title"
      >
        <v-card>
          <v-card-media
            :src="card.src"
            height="300px"
          >
            <v-container
              fill-height
              fluid
              pa-2
            >
              <v-layout fill-height>
                <v-flex xs12 align-end flexbox>
                  <!-- <span class="headline white--text" v-text="card.title"></span> -->
                </v-flex>
              </v-layout>
            </v-container>
          </v-card-media>

          <v-card-title>
            <div>
              <span class="grey--text">Number {{ index + 1 }}</span><br>
              <span v-text="card.title"></span><br>
              <span>Whitsunday Island, Whitsunday Islands</span>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon>favorite</v-icon>
            </v-btn>
            <v-btn icon>
              <v-icon>bookmark</v-icon>
            </v-btn>
            <v-btn icon>
              <v-icon>share</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      cards: [
        { title: 'Pre-fab homes', src: '/assets/img/invitation_gate_fold.jpg', flex: 4 },
        { title: 'Pre-fab homes', src: '/assets/img/invitation_elegance_white.jpg', flex: 4 },
        { title: 'Pre-fab homes', src: '/assets/img/invitation_gate.jpg', flex: 4 },
        { title: 'Pre-fab homes', src: '/assets/img/invitation_square_lace.jpg', flex: 4 },
        { title: 'Pre-fab homes', src: '/assets/img/invitation_square_lace.jpg', flex: 4 },
        { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 4 },
        { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 4 },
        { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 4 },
        { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 4 }
      ]
    })
  }
</script>

<style>

</style>
