<template>
  <div class="gallery">
    <h1>CONTACT US</h1>
        <div class="card">
          <img src='@/static/contact.png' alt="Card Image" />
          <div>
            <div class="text-card">
              <div>XFAS Marketing</div>
              <div>(+66) 89 767 2256</div>
              <div>xfas.marketing@gmail.com</div>
              <div>https://xfas.io</div>
              <div>@484ztjzf</div>
            </div>
            <div class="view-more">
              <button class="view-button">Book Now</button>
            </div>
          </div>
        </div>
       
  </div>
</template>

<script>
export default {
  name: 'Contact',

  data() {
    return {
 
    }
  }, 


}
</script>
<style scoped>
.gallery {
  padding:  40px 10px 40px 10px;
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
.text-card{
  display: flex;
  flex-direction: column;
  gap: 12px;
  align-items: left;
  color: var(--xfax-104-b-4-fd, #182432);
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
.card img {
  width:  300px;
  height: 400px;
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
  margin-top: 28px;
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
@media screen and (min-width: 640px) {
  .card {
    flex-direction: row;
    gap: 30px;
  }
  .text-card{
    width: 300px;
}
  .view-more {
  justify-content: left;
}
}
</style>
