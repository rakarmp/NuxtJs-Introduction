<template>
  <v-timeline>
    <v-timeline-item
      v-for="(year, i) in years"
      :key="i"
      :color="year.color"
      small
    >
      <template v-slot:opposite>
        <span
          :class="`headline font-weight-bold ${year.color}--text`"
          v-text="year.year"
        ></span>
      </template>
      <div class="py-4">
        <h2 :class="`headline font-weight-light mb-4 ${year.color}--text`">
          {{ year.title }}
        </h2>
        <div>
          {{ year.isi }}
        </div>
      </div>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
  export default {
    data: () => ({
      years: [
        {
          color: 'cyan',
          year: 'Laravel',
          title: 'Framework PHP',
          isi: 'kerangka kerja aplikasi web berbasis PHP yang sumber terbuka, menggunakan konsep Model-View-Controller. Laravel berada dibawah lisensi MIT, dengan menggunakan GitHub sebagai tempat berbagi kode.'
        },
        {
          color: 'green',
          year: 'Vue JS',
          title: 'The Progressive Javascript Framework',
          isi: ' kerangka kerja JavaScript yang bersifat progresif, bersumber terbuka untuk membangun antarmuka pengguna. Integrasi ke dalam proyek yang menggunakan pustaka JavaScript lainnya mudah dilakukan dengan Vue karena ia dirancang untuk bisa berjalan hanya di beberapa bagian halaman web.'
        },
        {
          color: 'pink',
          year: 'Nuxt JS',
          title: 'The Intuitive Vue Framework',
          isi: 'kerangka kerja aplikasi web yang bebas dan sumber terbuka berketergantungan pada Vue.js, Node.js, Webpack, dan Babel.js. Kerangka kerja ini dipromosikan sebagai "kerangka meta untuk aplikasi universal".'
        },
        {
          color: 'amber',
          year: 'CI 4',
          title: 'Framework PHP',
          isi: 'merupakan aplikasi sumber terbuka yang berupa kerangka kerja PHP dengan model MVC (Model, View, Controller) untuk membangun situs web dinamis dengan menggunakan PHP.'
        },
        {
          color: 'orange',
          year: 'React JS',
          title: 'A JavaScript Library',
          isi: 'Library JavaScript front-end sumber terbuka dan gratis untuk membangun antarmuka pengguna berdasarkan komponen UI.'
        },
      ],
    }),
  }
</script>

<style scoped>
h1 {
  font-size: 20px;
}
</style>
