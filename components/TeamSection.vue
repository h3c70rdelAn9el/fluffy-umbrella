<template>
  <div id="team-section">
    <h1 class="team-title p-1">
      Our Incredible Team!
    </h1>
    <b-container class="bv-row">
      <b-row>
        <b-col v-for="member in members" :key="member.name">
          <a href="#">
            <b-card
              class="card"
              :title="member.name"
              :sub-title="member.title"
              :img-src="member.img"
            >
              <b-card-text>
                {{ member.text }}
              </b-card-text>
            </b-card>
          </a>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  data () {
    return {
      members: [
        {
          name: 'Andre Stevapalo',
          title: 'Dev',
          text: 'Lorem ipsum dolor sit amet consectetur.',
          img: 'http://placebeard.it/680/480'
        },
        {
          name: 'El Beardo',
          title: 'Design-o',
          text: 'Ducimus eligendi exercitationem eaque ad voluptatum neque ullam quaerat doloremque eius.',
          img: 'http://placebeard.it/640/480'
        },
        {
          name: 'Bandito Azul',
          title: 'Marketing',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus fuga impedit illum?',
          img: 'http://placebeard.it/620/480'
        }
      ]
    }
  }
}
</script>

<style scoped>
  .team-title {
    text-align: center;
    color: rgb(159, 71, 202);
  }
  .bv-row {
    background-color: rgb(84, 26, 112);
    padding: 30px;
    border-radius: 10px;
  }

  #team-section {
    background-color: black;;
  }

  .card {
    min-height: 400px;
    margin: 5px;
  }

  .card img {
    height: 175px;
    padding: 10px;
    border-radius: 20px;
    object-fit: cover;
    object-position: center;
    transition: .5s;

  }

  .card img:hover {
    border-radius: 0px;
    transform: scale(1.1, 1.2);
  }
</style>
