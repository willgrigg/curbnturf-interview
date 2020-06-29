<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="drawerOpen = !drawerOpen"
        />

        <q-toolbar-title>
          Will Grigg
        </q-toolbar-title>
        <div class="text-subtitle1">{{ todaysDate }}</div>
      </q-toolbar>
    </q-header>

<q-drawer
        v-model="drawerOpen"
        show-if-above
        :width="220"
        :breakpoint="600"
        bordered
        content-class="bg-grey-3"
      >
        <q-scroll-area class="fit">
          <q-list padding>

            <q-item 
            to="/"
            exact
            clickable 
            v-ripple>
              <q-item-section avatar>
                <q-icon name="emoji_people"/>
              </q-item-section>
              <q-item-section>
                Intro
              </q-item-section>
            </q-item>
            <q-item 
            to="/examples"
            exact
            clickable
            v-ripple>
              <q-item-section avatar>
                <q-icon name="emoji_objects"/>
              </q-item-section>
              Examples
              <q-item-section>
              </q-item-section>
            </q-item>

          </q-list>
        </q-scroll-area>
      </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script> 

import { date } from 'quasar'
import EssentialLink from 'components/EssentialLink.vue'

export default {
  name: 'MainLayout',

  data () {
    return {
      drawerOpen: false
    }
  },
  computed: {
    todaysDate() {
      let timeStamp = Date.now(); 
      return date.formatDate(timeStamp, "dddd, MMMM Do");
    }
  },
  
}
</script>
