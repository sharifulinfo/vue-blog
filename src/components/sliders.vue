<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Slides with custom text -->
      <b-carousel-slide v-for="ss in sliders" v-bind:key="ss.img" :img-src="ss.img">
        <h1>Hello</h1>
      </b-carousel-slide>

    </b-carousel>
<div class="mb-2"></div>
  </div>
</template>

<script>
  export default {
    name : 'sliders',
    data() {
      return {
        slide: 0,
        sliding: null,
        sliders : [
          {img:'https://picsum.photos/1024/480/?image=53'},
          {img:'https://picsum.photos/1024/480/?image=54'},
          {img:'https://picsum.photos/1024/480/?image=55'},
          {img:'https://picsum.photos/1024/480/?image=56'},
        ]
      }
    },
    methods: {
      onSlideStart() {
        this.sliding = true
      },
      onSlideEnd() {
        this.sliding = false
      }
    }
  }
</script>