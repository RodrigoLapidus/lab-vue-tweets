<template>
  <div className="tweet">
    <ProfileImage :image="tweet.user.image"/>

    <div className="body">
      <div className="top">
        <User :userData="tweet.user" />
        <TimeStamp :time="tweet.timestamp" />
      </div>
      <Message :message="tweet.message" />
      <!--<Actions />-->
      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import TimeStamp from './TimeStamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

  
export default {
  name: "Tweet",

  components: {
    ProfileImage,
    User,
    TimeStamp,
    Message,
    Actions,
    },

  methods: {},

  computed: {},

  props: {
    tweet: Object,
  },

};


</script>

<style scoped>
a {
  color: #42b983;
}
</style>
