<template>
  <div class="gallery">
    <h1>OUR TEAM</h1>
    <v-row class="row-gallery">
      <v-col v-for="(card, index) in cards" :key="index" cols="6" sm="4" md="2">
        <div class="card">
          <img :src="card.img" alt="Card Image" />
          <div class="card-name">{{card.name}}</div>
          <div class="card-position">{{card.position}}</div>
          <div class="card-position">{{card.secposition}}</div>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'Team',
  data() {
    return {
      cards: [
        { img:  require('@/static/t1.png'),name: 'Chainuwat Manotam',position :'UNMANNED PILOT (UP)',},
        { img: require('@/static/t2.png'),name: 'Takurn Palawong',position :'UNMANNED PILOT (UP)', },
        { img: require('@/static/t3.png'),name: 'Sornrob Headkhuntod',position :'VISUAL OBSERVER (VO)', },
        {img: require('@/static/t4.png'),name: 'Thanaphat Khatawee',position :'UNMANNED PILOT (UP)',},  
        { img: require('@/static/t5.png'),name: 'Sornrob Headkhuntod',position :'UNMANNED PILOT (UP)' ,secposition :'COMMAND (UPIC) UU'  },
        { img: require('@/static/t6.png'),name: 'Donyarit Sakerm',position :'UNMANNED PILOT (UP)', },
      ],
    }
  },

}
</script>
<style scoped>
.gallery {
  padding:  40px 10px 40px 10px;
  border-radius: 0px 0px 16px 16px;
  background: #333;
}
.gallery h1 {
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
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  overflow: hidden;
  object-fit: cover;
  margin: auto;
  
}
.card-name {
text-align: center;
font-size: 12px;
font-style: normal;
font-weight: 500;
line-height: 96.523%; 
background: var(--Linear-1, linear-gradient(54deg, #04B4FD 3.46%, #4EDAFD 92.22%));
background-clip: text;
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
margin-top: 12px;
margin-bottom: 4px;
}
.card-position {
color: var(--FFFFFF, #FFF);
text-align: center;
font-family: Inter;
font-size: 10px;
font-style: normal;
font-weight: 300;
line-height: 96.523%; /* 9.652px */
align-self: stretch;
}
.card img {
 width:  100px;
  height: 100px;
  border-radius: 999px;
  object-fit: cover;
}
.col-6,
.col-4 {
  padding: 10px;
}

</style>
