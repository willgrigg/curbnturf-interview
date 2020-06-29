<template>
  <q-page class="q-pa-lg">
    <h3 class="q-mt-none"><strong>A Few Examples</strong></h3>
    <h5><em><u>Websites (created with Jekyll):</u></em>
    </h5>
    <q-div class="float-left">
    <a href="https://www.madebymikayla.com">
    <img border="0" src="madebymikayla.png" width="100" height="100"/></a>
    <p><em>MadeByMikayla.com: a website I made for my roommate. Hosted on Netlify.</em></p>
    <a href="https://www.willwgrigg.com">
    <img border="0" src="me.jpg" width="100" height="100"/></a>
    <p><em>WillWGrigg.com: a webpage I created to host my resume publicly. Hosted on Netlify.</em></p>
    </q-div>
    <q-div class="float-left">
    <h5><em><u>Other CS Projects:</u></em></h5>
    <ul>
    <li><a href="https://github.com/edwardsjohnmartin/htopics">
    A Python project I worked on at Idaho State University. Scraped tweets from Twitter and created networks based on perceived strength of word association.</a>
    </li>
    <li><a href="https://github.com/edwardsjohnmartin/3PIO">
    Another ISU project. Essentially an in-house Codecademy -- I wrote the backend grading logic for this in Python.</a>
    </li>
    <li>
    <a href="https://github.com/willgrigg/woodgrain-statcounter">
    A small C# application I wrote when I was at Woodgrain. Gathers statistics automatically at the end of each shift -- used 3 times a day to this day!</a>
    </li>
    </ul>
    </q-div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex'
}
</script>
