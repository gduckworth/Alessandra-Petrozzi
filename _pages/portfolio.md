---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: false
sidebar:
  nav: "sidenav"
---

<script src="https://unpkg.com/vue"></script>
<script src="https://unpkg.com/vue-instagram"></script>

<script src="ism/js/ism-2.2.min.js"></script>

<template>
  <vue-instagram token="bfd5aafc0a674124a18ba1caecd02300" :count="5" : mediaType="image">
    <template slot="feeds" slot-scope="props">
      <li class="fancy-list"> {{ props.feed.link }} </li>
    </template>
    <template slot="error" slot-scope="props">
      <div class="fancy-alert"> {{ props.error.error_message }} </div>
    </template>
  </vue-instagram>
</template>

<script>
import VueInstagram from 'vue-instagram'

export default {
  name: 'App',

  components: {
    VueInstagram
  }
}
</script>