<template>
  <section id="project" class="project">
    <Project width="width: 40%">
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>oui oui</h1>
      <p>Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
    </template>
    </Project>
    <Project   width="width: 40%">
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>oui oui</h1>
      <p>Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
    </template>
    </Project>
    <Project   width="width: 33.33%">
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>oui oui</h1>
      <p>Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
    </template>
    </Project>
    <Project   width="width: 33.33%">
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>oui oui</h1>
      <p>Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
    </template>
    </Project>
    <Project   width="width: 33.33%">
    <template v-slot:img>
      <img src="https://media-cdn.tripadvisor.com/media/photo-s/09/2b/37/3c/ocean-blue-tenerife.jpg" alt="preview site"/>
    </template>
    <template v-slot:text>
      <h1>oui oui</h1>
      <p>Ipsum enim sunt nesciunt minus id Ratione similique minus dolor nobis commodi Nisi tenetur similique?</p>
    </template>
    </Project>
  </section>
</template>

<script>
import Project from './Project.vue';

export default{
  name: 'Projects',
  components: {
    Project
  }
}
</script>

<style scoped>
.project {
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}

</style>

