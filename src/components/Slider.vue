<template>
  <div
    class="p-5"
    style="background-image: url('https://blog.walls.io/wp-content/uploads/2017/02/ideas-for-making-event-more-social.jpg'); width: 100%;
    height: 660px;"
    id="etkinlikler"
  >
  <!-- <img src="https://www.digitalsme.eu/digital/uploads/Untitled-design-4.png" class="resim"/> -->
    <div class="container" >
      <transition-group name="fade" tag="div">
        <div class="container" v-for="i in [currentIndex]" :key="i">
          <img :src="currentImg" class="ab" />
        </div>
      </transition-group>
      <a class="prev" @click="prev">&#10094; Önceki</a>
      <a class="next" @click="next">&#10095; Sonraki</a>
    </div>
  </div>
</template>
<script>
export default {
  name: "Slider",
  data() {
    return {
      images: [
        "https://cdn.pixabay.com/photo/2015/12/12/15/24/amsterdam-1089646_1280.jpg",
        "https://cdn.pixabay.com/photo/2016/02/17/23/03/usa-1206240_1280.jpg",
        "https://cdn.pixabay.com/photo/2015/05/15/14/27/eiffel-tower-768501_1280.jpg",
        "https://cdn.pixabay.com/photo/2016/12/04/19/30/berlin-cathedral-1882397_1280.jpg",
      ],
      timer: null,
      currentIndex: 0,
    };
  },

  mounted: function() {
    this.startSlide();
  },

  methods: {
    startSlide: function() {
      // this.timer = setInterval(this.next, 4000);
    },

    next: function() {
      this.currentIndex += 1;
    },
    prev: function() {
      this.currentIndex -= 1;
    },
  },

  computed: {
    currentImg: function() {
      return this.images[Math.abs(this.currentIndex) % this.images.length];
    },
  },
};
</script>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: all 0.9s ease;
  overflow: hidden;
  visibility: visible;
  position: absolute;
  width: 100%;
  opacity: 1;
}

.fade-enter,
.fade-leave-to {
  visibility: hidden;
  width: 100%;
  opacity: 0;
}

img {
  height: 600px;
  width: 100%;
}

.prev,
.next {
  cursor: pointer;
  position: absolute;
  top: 250%;
  width: auto;
  padding: 16px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.7s ease;
  border-radius: 0 4px 4px 0;
  text-decoration: none;
  user-select: none;
}

.next {
  right: 10%;
}

.prev {
  left: 10%;
}

.prev:hover,
.next:hover {
  background-color: #bf1e2d;
}
.arkaplan {
    position: relative;
    overflow: hidden;
    padding: 16px;
    height: 660px;
}
.resim {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: auto;
    opacity: 0.6;
}
</style>
