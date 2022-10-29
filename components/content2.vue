<template>
     <v-row
    align="center"
    justify="center"
  >
    <v-col cols="12">
      <v-hover
        v-slot="{ hover }"
        disabled
      >
        <v-card
          :elevation="hover ? 12 : 2"
          class="mx-auto"
          height="350"
          max-width="200vh"
        >
          <v-card-text class="my-4 text-left text-h6">
            Hi I'm Raka, let me introduce myself, I was born in Bandung on the 12th, I studied from elementary until now at SMA Assalaam Bandung, thank you, maybe just like that, I hope you like it
          </v-card-text>
        </v-card>
      </v-hover>
    </v-col>
  </v-row>
</template>

<script>
export default {
    name: 'isi'
}
</script>