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
      <div v-for="image in images" :key="image.id">
        <b-carousel-slide
          :caption="image.caption"
          :text="image.text"
          :img-src="image.src"
        >
          <p>
            {{ image.content }}
          </p>
        </b-carousel-slide>
        <!-- Text slides with image -->

        <!-- Slides with custom text -->
        <!-- <img-src="https://picsum.photos/1024/480/?image=54" />
        <h1>Custom text</h1>
        <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=58" />
      </div> -->

        <!-- Slides with image only -->

        <!-- Slides with img slot -->
        <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
        <!-- <b-carousel-slide>
          <template #img>
            <img
              class="d-block img-fluid w-100"
              width="1024"
              height="480"
              src="https://picsum.photos/1024/480/?image=55"
              alt="image slot"
            >
          </template>
        </b-carousel-slide> -->

        <!-- Slide with blank fluid image to maintain slide aspect ratio -->
        <!-- <b-carousel-slide caption="Blank Image" img-blank img-alt="Blank image">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
            a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
          </p>
        </b-carousel-slide> -->
      </div>
    </b-carousel>
  </div>
</template>

<script>
export default {
  data () {
    return {
      slide: 0,
      sliding: null,
      images: [
        {
          caption: 'First slide',
          text: 'Nulla vitae elit libero, a pharetra augue mollis interdum.',
          src: 'https://picsum.photos/1024/480/?image=52',
          content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.'
        },
        {
          caption: 'Second slide',
          text: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Earum, incidunt.',
          src: 'https://picsum.photos/1024/480/?image=62'
        },
        {
          caption: 'Third slide',
          text: 'Qui nihil quaerat itaque sunt ex error minima dolorem distinctio velit',
          src: 'https://picsum.photos/1024/480/?image=64',
          content: 'Quibusdam culpa, voluptatibus deserunt molestiae earum similique odit magnam.Cum, quam perferendis. Necessitatibus similique praesentium sapiente molestiae!'
        }
      ]
    }
  },
  methods: {
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }
}
</script>
