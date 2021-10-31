<template>
  <div class="wrapper">
    <div class="content-div">
      <div class="content">
        <div
          class="img-div"
          :style="`background-image: url(${require('~/assets/images/bitcoin.png')})`"
        ></div>
        <span class="selected"></span>
        <div class="content-wrapper container">BITCOIN</div>
      </div>
      <div class="content">
        <div
          class="img-div"
          :style="`background-image: url(${require('~/assets/images/etherum.png')})`"
        ></div>
        <span class="selected"></span>
        <div class="content-wrapper container">ETHERNUM</div>
      </div>
      <button v-ripple class="">Compare</button>
    </div>
    <div class="func-wrapper">
      <div class="func-div">
        <div class="scroll-btn"></div>
        <div class="container">
          <div>
            <h3>MARKET CAP</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum
              aliquid error quae fugit velit rerum. Magni laudantium, cumque
              consectetur sint laborum voluptatibus! Accusantium inventore ipsam
              hic molestiae ut facilis sequi!
            </p>
          </div>
          <div>
            <h3>TOTAL SUPPLY</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum
              aliquid error quae fugit velit rerum. Magni laudantium, cumque
              consectetur sint laborum voluptatibus! Accusantium inventore ipsam
              hic molestiae ut facilis sequi!
            </p>
          </div>
          <div>
            <h3>CIRCULATING SUPPLY</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum
              aliquid error quae fugit velit rerum. Magni laudantium, cumque
              consectetur sint laborum voluptatibus! Accusantium inventore ipsam
              hic molestiae ut facilis sequi!
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Index'
}
</script>

<style scoped>
.wrapper {
  display: flex;
  align-items: center;
}
.content-div {
  width: 100%;
}
.content {
  display: flex;
  position: relative;
  margin: 2rem auto;
  background: #2e2e2e;
  min-height: 200px;
  width: 90%;
  border-radius: 1rem;
}
.content-wrapper {
  position: absolute;
  right: 1rem;
  bottom: 1rem;
  font-weight: 600;
  font-size: 1.2rem;
  width: 100%;
  display: flex;
  justify-content: end;
}
.selected {
  position: absolute;
  right: 1rem;
  top: 1rem;
  background: #06d6a0;
  border-radius: 50%;
  width: 15px;
  height: 15px;
}
.img-div {
  position: absolute;
  background-repeat: no-repeat;
  background-position-x: -37px;
  background-position-y: 70px;
  background-clip: border-box;
  background-size: 180px;
  width: inherit;
  height: 100%;
  border-radius: 0 0 0 1rem;
}
.content-div button {
  margin: 0 auto;
  display: flex;
  width: 50%;
  background: #06d6a0;
  color: #fafafa;
  padding: 0.8rem;
  border-radius: 1rem;
  justify-content: center;
  font-size: 1rem;
  box-shadow: 0px 0px 15px 0 rgba(6, 214, 160, 0.5);
  /* font-weight: 500; */
}
.func-wrapper {
  position: fixed;
  min-height: 100vh;
  top: 5%;
  bottom: 0;
  padding-top: 85vh;
  width: 95%;
  max-width: 768px;
  margin: 0 auto;
  overflow-y: scroll;
  left: 0;
  right: 0;
}
.func-div {
  background: #2e2e2e;
  margin: 0 auto;
  border-radius: 1rem 1rem 0 0;
  padding: 1rem 0.5rem;
}
.func-div .scroll-btn {
  display: block;
  background: #fafafa;
  width: 100px;
  height: 10px;
  border-radius: 1rem;
  margin: 0.5rem auto;
}
/* .func-div .container {
} */
</style>
