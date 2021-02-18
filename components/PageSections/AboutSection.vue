<template>
  <div id="about-section">
    <h1 class="py-2 about-section__title">
      Little About Us
    </h1>
    <b-row class="about-section__content">
      <b-col class="left-content">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, perferendis quia? Iste non facere adipisci et, facilis eveniet unde quod!</p>
      </b-col>
      <b-col class="right-content">
        <div class="image-section">
          <img src="https://picsum.photos/1024/480/?image=65" alt="aboutpic" class="about-img">
        </div>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Accusantium commodi nemo cum dolores esse modi delectus excepturi! Excepturi, ullam inventore.</p>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.about-section__title {
  background-color: rgb(165, 159, 159);
  text-align: center;
}

.about-section__content {
  background: rgb(131,58,180);
  background: linear-gradient(175deg, rgba(131,58,180,1) 0%, rgba(121,93,124,1) 47%, rgba(10,10,10,1) 90%);
  color: white;
  margin-top: -10px;
  padding: 10px;
}

.left-content {
  margin-top: 40px;
  text-align: center;
}

.image-section {
  display: flex;
}

.about-img {
  height: 150px;
  padding: 10px;
  margin: 0 auto 0 auto;
  border-radius: 20px;
  box-shadow: 0px 0px 10px gray;
}

</style>
