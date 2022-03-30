<template>
  <v-container id="overview">
    <v-row justify="center" align="center" class="mb-5">
      <v-col cols="6" sm="12" md="6">
        <v-img
          class="rounded-lg elevation-2"
          contain
          src="/showcase1.png"/>
      </v-col>
      <v-col cols="6" sm="12" md="6" class="justify-start">
        <h1>
          All your migrations in one place!
        </h1>
        <p>
          Ef Steriod is a tool for managing your Entity Framework migrations at a glance.
          Entity Framework core and Entity Framework 6 are supported out of the box!
        </p>
      </v-col>
    </v-row>
    <v-row justify="center" align="center" class="mb-5">
      <v-col cols="6" sm="12" md="6" class="justify-start">
        <h1>
          Multi-DB context support
        </h1>
        <p>
          Select which DB context to use for your migrations with one click and switch between them with ease.
        </p>
      </v-col>
      <v-col cols="6" sm="12" md="6">
        <v-img
          class="rounded-lg elevation-2"
          contain
          src="/DbContext.png"/>
      </v-col>
    </v-row>
    <v-row justify="center" align="center" class="mb-5">
      <v-col cols="6" sm="12" md="6">
        <v-img
          class="rounded-lg elevation-2"
          contain
          src="/features.png"/>
      </v-col>
      <v-col cols="6" sm="12" md="6" class="justify-start">
        <h1>
          Feature packed!
        </h1>
        <p>
          List, delete, update, target migration, and more!
          Different project in different tabs! multi task with ease!
          And we are still working on more features!
          Check out our GitHub repo for more information!
        </p>
      </v-col>
    </v-row>

    <v-row justify="center" align="center" id="download">
      <v-btn color="secondary" class="mb-5 mr-3" href="https://github.com/Ef-Steroid/ef_steroid/releases" elevation="0">
        Download on Github
      </v-btn>
      <v-btn color="secondary" class="mb-5" href="https://github.com/Ef-Steroid/ef_steroid/releases" elevation="0">
        Download on Microsoft Store
      </v-btn>
    </v-row>

    <v-container id="faqs">
      <h1>FAQs</h1>
      <v-row justify="center" align="center" class="mt-2">
        <v-expansion-panels>
          <v-expansion-panel>
            <v-expansion-panel-header color="#1F2832">
              <h3>Why did we make this tool?</h3>
            </v-expansion-panel-header>
            <v-expansion-panel-content color="#1F2832">
              We use Entity Framework core and Entity Framework 6 regularly and we wanted to make a tool that is easy to use and easy to use for everyone.
            </v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel>
            <v-expansion-panel-header color="#1F2832">
              <h3>What technologies do you use?</h3>
            </v-expansion-panel-header>
            <v-expansion-panel-content color="#1F2832">
              Flutter, SqlLite, and C++.
            </v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel>
            <v-expansion-panel-header color="#1F2832">
              <h3>How do I contribute to this project? </h3>
            </v-expansion-panel-header>
            <v-expansion-panel-content color="#1F2832">
              Please check out our GitHub repo for contribution guidelines.
            </v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel>
            <v-expansion-panel-header color="#1F2832">
              <h3>Can do I request a feature or raise an issue?</h3>
            </v-expansion-panel-header>
            <v-expansion-panel-content color="#1F2832">
              Please use our GitHub repo for issues and feature requests.
            </v-expansion-panel-content>
          </v-expansion-panel>
        </v-expansion-panels>
      </v-row>
    </v-container>

  </v-container>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
