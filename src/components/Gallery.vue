<template>
  <v-container>
  <v-layout
    row
    wrap
    class="my-5"
    align-center
  >
    <v-flex xs12 sm6 lg4>
      <v-card hover class="mr-2 mt-2">
        <v-card-media
          class="black--text"
          height="250px"
          src="/assets/invitation_church_red.png"
        >
          <v-container fill-height fluid>
            <v-layout fill-height>
              <v-flex xs12 align-end flexbox>
                <!-- <span class="headline">Invitation church</span> -->
              </v-flex>
            </v-layout>
          </v-container>
        </v-card-media>
        <v-card-title>
          <div>
            <span class="grey--text">No.2</span><br>
            <div class="headline">Wedding invitation lace</div>
            <p>
              Wedding invitations card laser cut. With inner sheet and envelope.</p> 

            
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat @click="show = !show" color="orange">Info</v-btn>
          <v-spacer></v-spacer>
          <v-btn icon @click="show = !show">
            <v-icon color="orange">{{ show ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
          </v-btn>
        </v-card-actions>

        <v-slide-y-transition>
          <v-card-text v-if="show">
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
    <v-flex xs12 sm6 lg4>
      <v-card hover class="mr-2 mt-2">
        <v-card-media
          class="black--text"
          height="250px"
          src="/assets/img/invitation_elegance_white.jpg"
        >
          <v-container fill-height fluid>
            <v-layout fill-height>
              <v-flex xs12 align-end flexbox>
                <!-- <span class="headline">Invitation church</span> -->
              </v-flex>
            </v-layout>
          </v-container>
        </v-card-media>
        <v-card-title>
          <div>
            <span class="grey--text">No.2</span><br>
            <div class="headline">Wedding invitation lace</div>
            <p>
              Wedding invitations card laser cut. With inner sheet and envelope.</p> 

            
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat @click="show = !show" color="orange">Info</v-btn>
          <v-spacer></v-spacer>
          <v-btn icon @click="show = !show">
            <v-icon color="orange">{{ show ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
          </v-btn>
        </v-card-actions>

        <v-slide-y-transition>
          <v-card-text v-if="show">
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
    <v-flex xs12 sm6 lg4>
      <v-card hover class="mr-2 mt-2">
        <v-card-media
          class="black--text"
          height="250px"
          src="/assets/img/invitation_elegance_white.jpg"
        >
          <v-container fill-height fluid>
            <v-layout fill-height>
              <v-flex xs12 align-end flexbox>
                <!-- <span class="headline">Invitation church</span> -->
              </v-flex>
            </v-layout>
          </v-container>
        </v-card-media>
        <v-card-title>
          <div>
            <span class="grey--text">Number 10</span><br>
            <span>Invitation church</span><br>
            <span>Whitsunday Island, Whitsunday Islands</span>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 lg4 >
      <v-card hover class="mr-2 mt-2">
        <v-card-media
          class="black--text"
          height="250px"
          src="/assets/img/invitation_gate_fold.jpg"
        >
          <v-container fill-height fluid>
            <v-layout fill-height>
              <v-flex xs12 align-end flexbox>
                <!-- <span class="headline">Invitation church</span> -->
              </v-flex>
            </v-layout>
          </v-container>
        </v-card-media>
        <v-card-title>
          <div>
            <span class="grey--text">Number 10</span><br>
            <span>Invitation church</span><br>
            <span>Whitsunday Island, Whitsunday Islands</span>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
        <v-flex xs12 sm6 lg4>
      <v-card hover class="mr-2 mt-2">
        <v-card-media
          class="black--text"
          height="250px"
          src="/assets/img/invitation_gate.jpg"
        >
          <v-container fill-height fluid>
            <v-layout fill-height>
              <v-flex xs12 align-end flexbox>
                <!-- <span class="headline">Invitation church</span> -->
              </v-flex>
            </v-layout>
          </v-container>
        </v-card-media>
        <v-card-title>
          <div>
            <span class="grey--text">Number 10</span><br>
            <span>Invitation church</span><br>
            <span>Whitsunday Island, Whitsunday Islands</span>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 lg4>
      <v-card hover class="mr-2 mt-2">
        <v-card-media
          class="black--text"
          height="250px"
          src="/assets/img/invitation_square_lace.jpg"
        >
          <v-container fill-height fluid>
            <v-layout fill-height>
              <v-flex xs12 align-end flexbox>
                <!-- <span class="headline">Invitation church</span> -->
              </v-flex>
            </v-layout>
          </v-container>
        </v-card-media>
        <v-card-title>
          <div>
            <span class="grey--text">Number 10</span><br>
            <span>Invitation church</span><br>
            <span>Whitsunday Island, Whitsunday Islands</span>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 lg4>
      <v-card hover class="mr-2 mt-2">
        <v-card-media
          class="black--text"
          height="250px"
          src="/assets/img/invitation_square_with_ribbon.jpg"
        >
          <v-container fill-height fluid>
            <v-layout fill-height>
              <v-flex xs12 align-end flexbox>
                <!-- <span class="headline">Invitation church</span> -->
              </v-flex>
            </v-layout>
          </v-container>
        </v-card-media>
        <v-card-title>
          <div>
            <span class="grey--text">Number 10</span><br>
            <span>Invitation church</span><br>
            <span>Whitsunday Island, Whitsunday Islands</span>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      show: false
    })
  }
</script>

<style>

</style>
