<template>
  <v-container
    grid-list-lg
  >
    <v-layout row wrap>
      <v-flex
        xs12
        sm6
        xl3
        v-for="(card, index) in cards"
        v-bind="{ [`lg${card.flex}`]: true }"
        :key="card.id"
      >
        <v-card hover>
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
              <span v-text="card.description">No description</span>
            </div>
          </v-card-title>

          <v-card-actions>
            <!-- <v-btn flat @click="show = !show" color="orange">Info</v-btn> -->
            <v-btn flat @click="showMore(index)" color="orange">Info</v-btn>
            <v-spacer></v-spacer>
            <v-btn @click="showMore" icon>
              <v-icon>favorite</v-icon>
            </v-btn>
            <v-btn icon>
              <v-icon>bookmark</v-icon>
            </v-btn>
            <v-btn icon>
              <v-icon>share</v-icon>
            </v-btn>
            <v-btn icon @click="show = !show">
              <v-icon color="orange">{{ show ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
            </v-btn>
          </v-card-actions>
          <v-slide-y-transition>
            <v-card-text ref="index" v-if="show">
              <span>It is high-grade paper, 200g. Size: 127*186mm. </span><br>
              ​<span class="grey--text">
                Available colours: white / dark blue / white / beige / black / see color board
              </span>
              <div>Order quantity: </div>
              <div>
                <li>min 10 items Eur 6 each</li>
                <li>11-20 items Eur 5 each</li>
                <li>21-30 items Eur 4.5 each</li>
                <li>31 up items  Eur 4 each</li>
              </div>
              
            </v-card-text>
          </v-slide-y-transition>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    methods: {
      showMore: function(index){
        this.show = !this.show
        console.log('clicked ' + index)
      }
    },
    data: () => ({
      show: false,
      cards: [
        {
          title: 'Pre-fab homes',
          src: '/assets/img/invitation_gate_fold.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Pre-fab homes',
          src: '/assets/img/invitation_elegance_white.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Pre-fab homes',
          src: '/assets/img/invitation_gate.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Pre-fab homes',
          src: '/assets/img/invitation_square_lace.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Pre-fab homes',
          src: '/assets/img/invitation_square_lace.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Favorite road trips',
          src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Favorite road trips',
          src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Best airlines',
          src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg',
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        },
        {
          title: 'Best airlines',
          src: "`https://unsplash.it/300/300?image=${Math.floor(Math.random() * 100) + 1}`",
          flex: 4,
          description: 'Wedding invitations card laser cut. With inner sheet and envelope.',
        }
      ]
    })
  }
</script>

<style>

</style>
