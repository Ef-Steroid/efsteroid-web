<template>
  <v-app dark>
    <v-app-bar color="#1F2832" :clipped-left="clipped" fixed app elevation="0">
      <v-img
        class="mx-2"
        src="/logo.png"
        max-height="40"
        max-width="40"
        contain
      ></v-img>
      <v-toolbar-title v-text="title"/>
      <v-spacer/>
      <v-btn href="#overview" color="transparent" elevation="0">
        Overview
      </v-btn>
      <v-btn href="#download" color="transparent" elevation="0">
        Download
      </v-btn>
      <v-btn href="#faqs" color="transparent" elevation="0">
        FAQs
      </v-btn>
      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-btn color="transparent" elevation="0" href="https://github.com/Ef-Steroid/ef_steroid"
                 v-bind="attrs"
                 v-on="on">
            <v-icon>mdi-star</v-icon>
          </v-btn>
        </template>
        <span>Star us on Github</span>
      </v-tooltip>

    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt/>
      </v-container>
    </v-main>
    <v-footer :absolute="!fixed" app>
      <span>main contributor: </span> <a href="https://github.com/TabooSun">@taboosan </a>

      <span>&nbsp; &copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'EF Steroid',
    }
  },
}
</script>

