<template>
  <div class="home">
    <app-bar left="camera"
             right="paper-plane"
             title="Instagram"
             @left="toggleCamera"></app-bar>
    <navigation></navigation>
    <friend-list></friend-list>
    <feed-list></feed-list>
    <bottom-tabs></bottom-tabs>
    <camera></camera>
  </div>
</template>

<script>
import { mapMutations } from 'vuex'
import AppBar from '../components/AppBar'
import Navigation from '../components/Navigation'
import FriendList from '../components/FriendList'
import FeedList from '../components/FeedList'
import BottomTabs from '../components/BottomTabs'
import Camera from '../components/Camera'
export default {
  components: {
    AppBar,
    Navigation,
    FriendList,
    FeedList,
    BottomTabs,
    Camera
  },
  methods: {
    ...mapMutations(['toggleCamera'])
  }
}
</script>

<style lang="scss">
.home {
  padding-top: 88px;
  padding-bottom: 88px;
  width: 100%;
  min-height: calc(100vh - 88px - 64px);
  overflow: hidden;
  background-color: white;
  color: #333;
}
</style>