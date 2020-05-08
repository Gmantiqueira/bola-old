<template>
  <v-layout text-center wrap>
    <v-flex class="flex-row flex-wrap" layout xs12>
      <Bola
        class="my-5"
        v-for="bola in bolas"
        :key="bola.id"
        :imgLink="bola.link"
        :title="bola.title"
      ></Bola>
    </v-flex>
  </v-layout>
</template>

<script>
import Bola from '@/components/Bola'
import Jabulani from '@/assets/jabulani.jpg'
import Golf from '@/assets/golf.jpg'
import Baseball from '@/assets/baseball.jpg'
import Tenis from '@/assets/tenis.jpg'
import RocketLeague from '@/assets/rocket-league.jpg'

export default {
  components: { Bola },
  data: () => ({
    bolas: [
      {
        link: Jabulani,
        id: 1,
        title: 'Jabulani'
      },
      {
        link: Golf,
        id: 2,
        title: 'Golf'
      },
      {
        link: Baseball,
        id: 3,
        title: 'Baseball'
      },
      {
        link: Tenis,
        id: 4,
        title: 'Tenis'
      },
      {
        link: RocketLeague,
        id: 5,
        title: 'Rocket League'
      }
    ]
  })
}
</script>
