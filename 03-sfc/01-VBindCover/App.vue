<template>
  <div class="sample">
    <h1 style="text-align: center">С изображением</h1>
    <MeetupCover :title="meetupWithImage.title" :image="meetupWithImage.image"/>

    <h1 style="text-align: center">Без изображения</h1>
    <MeetupCover :title="meetupWithoutImage.title" :image="meetupWithoutImage.image"/>
  </div>
</template>

<script>
import MeetupCover from './components/MeetupCover.vue';

export default {
  name: 'App',

  components: {MeetupCover},

  data() {
    return {
      meetupWithImage: {
        title: 'VueConf US',
        image: 'https://course-vue.javascript.ru/api/images/5',
      },

      meetupWithoutImage: {
        title: 'Demo meetup',
        image: null,
      },
    };
  },
};
</script>

<style></style>
