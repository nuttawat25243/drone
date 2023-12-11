<template>
  <div class="gallery">
    <div class="logo-container">
    <img src='@/static/xfas-nav.png' alt="Card Image" />
    </div>
        <div class="card">
          <div class="text-card">
              <h1>NAVIGATOR</h1>
              <div class="nav-menu">
                <ul>Home</ul>
                <ul>Introduction</ul>
                <ul>Our Service</ul>
                <ul>Overview</ul>
                <ul>Package</ul>
                <ul>Drone Box</ul>
                <ul>Gallery</ul>
                <ul>Our Team</ul>
              </div>
          </div>
        </div>
  </div>
</template>

<script>
export default {
  name: 'Navigator',
}
</script>
<style scoped>
.logo-container{
  display: flex;
  justify-content: end;
}
.gallery {
  display: flex;
  flex-direction: column;
  padding:  5px 5px 40px 5px;
  background: var(--xfax-104-b-4-fd, #182432);
}
.logo-container img{
    width: 65px;
    height: 28px;
}
.text-card  {
  padding: 0 15px 0 15px;
}
.text-card h1 {
color: var(--xfax-1-fafafa, #FAFAFA);
font-family: Inter;
font-size: 20px;
font-style: normal;
font-weight: 600;
line-height: normal;
margin: 15px 0 12px 0 ;
}
.text-card ul{
  display: flex;
  flex-direction: column;
  gap: 8px;
  color: #999;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
@media screen and (min-width: 600px) {
            .nav-menu {
                display: flex;
                flex-wrap: wrap; 
            }

            .nav-menu ul {
                width: 50%;
            }
            .gallery {
                display: flex;
                flex-direction: row-reverse;
                justify-content: center;
                gap: 144px;
               
            }
            .gallery img{
                margin-top: 12px;
                width: 124px;
                height: 42px;

            }
}

</style>
