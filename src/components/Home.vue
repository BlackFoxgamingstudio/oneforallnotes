<template>
  <div class="container">
    <div style="width: 930px; margin: 0 auto;">
      <GridView></GridView>
      <div style="background: #FCE4EC; text-align: center; padding: 50px; margin: 50px 0; border-radius: 5px;">
        <h4> A modern Study Guide <strong>Lexi-kun</strong> using <strong>OneForAll as a Backend</strong> </h4>
        <div> Check out same project built with OneForAll
           <strong><a href="http://oneforall-224822.appspot.com/projects/" target="_blank">BlackFox OneForAll</a></strong>
        </div>
        <div> This R&amp;D project is developed to test grid-layout library for 
          <strong> <a href="http://oneforall-224822.appspot.com/Storyboards/5cdb3809cda9320ed07725d7/" target="_blank"> OneForAll StoryBoard </a></strong>.
        </div>
        <div> Next you can make a python library using <strong><a href="http://oneforall-224822.appspot.com/codes/test" target="_blank"> The StoryCode CLI </a></strong>. </div>
      </div>
    </div>
  </div>
</template>

<script>
import { mapActions } from 'vuex'
import GridView from './editor/GridView'

export default {
  name: 'home',
  components: { GridView },
  methods: {
    ...mapActions({
      fetchResources: 'fetchResources'
    })
  },
  created () {
    this.fetchResources()
  }
}
</script>
