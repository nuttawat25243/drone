<template>
  <div class="gallery">
    <h1>PACKAGES</h1>
    <p>Let’s get a new experience with our service.
       You can get more angle views that you want. Let’s see our packages.</p>

    <div class="view-more">
      <button class="view-button">View More</button>
    </div>
  </div>
</template>

<script>

export default {
 
  data() {
    return {
      cards: [
        { img: this.getRandomImage() },
        { img: this.getRandomImage() },
        { img: this.getRandomImage() },
        {
          img: 'https://dynamic-media-cdn.tripadvisor.com/media/photo-o/0f/ba/29/5c/img-worlds-of-adventure.jpg?w=1200&h=-1&s=1',
        },
        { img: this.getRandomImage() },
        { img: this.getRandomImage() },
      ],
    };
  },
  methods: {
    getRandomImage() {
      const width = 1123;
      const height = 1123;
      const randomImageId = Math.floor(Math.random() * 1000);
      return `https://source.unsplash.com/random/${width}x${height}?sig=${randomImageId}`;
    },
  },
};
</script>
<style scoped>
.gallery {
  margin: 40px 10px 40px 10px;
}
.gallery h1{
  display: flex;
  justify-content: center;
  text-align: center;
  font-size: 20px;
  font-style: normal;
  font-weight: 600;
  line-height: 96.523%; /* 19.305px */
  background: var(
    --Linear-1,
    linear-gradient(54deg, #04b4fd 3.46%, #4edafd 92.22%)
  );
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-bottom: 18px;
}
.row-gallery {
  margin: 0px;
}

.card {
  margin: auto;
  box-shadow: none !important;
  overflow: hidden;
  object-fit: cover;
  width: 100%;
  height: 120px;
  border-radius: 8px;
}

.card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.col-6,
.col-4 {
  padding: 10px;
}
.view-more {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 18px;
}
.view-button {
  display: flex;
  width: 167px;
  height: 36px;
  padding: 10px 16px;
  justify-content: center;
  align-items: center;
  border-radius: 16px;
  border: 1px solid var(--Linear-1, #04b4fd);
  background: var(--FFFFFF, #fff);
  box-shadow: 2px 2px 20px 0px rgba(0, 0, 0, 0.1);
  text-align: center;
  font-size: 12px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  letter-spacing: 0.54px;
  background: linear-gradient(54deg, #04b4fd 3.46%, #4edafd 92.22%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
@media screen and (min-width: 420px) {
  .card {
    height: 180px; 
  }
  .gallery {
  margin: 40px 20px 40px 20px;
}
}
@media screen and (min-width: 700px) {
  .card {
    height: 240px; 
  }
    .gallery {
  margin: 40px 40px 40px 40px;
}
}
@media screen and (min-width: 1200px)  {
  .card {
    height: 350px; 
  }
}
</style>
