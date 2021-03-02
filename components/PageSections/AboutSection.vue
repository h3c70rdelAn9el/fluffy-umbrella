<template>
  <div id="about-section">
    <h1 class="about-section__title pt-2">
      Little About Us
    </h1>
    <b-row class="about-section__content container">
      <b-col class="left-content">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, perferendis quia? Iste non facere adipisci et, facilis eveniet unde quod!</p>
      </b-col>
      <b-col class="right-content">
        <div class="image-section">
          <img src="https://picsum.photos/1024/480/?image=65" alt="aboutpic" class="about-img">
        </div>
        <p class="pt-2">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Accusantium commodi nemo cum dolores esse modi delectus excepturi! Excepturi, ullam inventore.
        </p>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {

}
</script>

<style>
#about-section {
  background: rgb(131,58,180);
  background: linear-gradient(175deg, rgba(131,58,180,1) 0%, rgba(121,93,124,1) 47%, rgba(10,10,10,1) 90%);
}

.about-section__title {
  text-align: center;
}

.about-section__content {
  color: white;
  /* padding: 10px; */
  /* width: 100%; */
}

.left-content {
  /* margin-top: 40px; */
  /* text-align: center; */
}

.image-section {
  display: flex;
}

.about-img {
  height: 150px;
  padding: 10px;
  border-radius: 20px;
  box-shadow: 0px 0px 10px gray;
}

</style>
