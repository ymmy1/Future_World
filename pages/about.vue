<template>
  <div class="home">
    <my-header>
      <h1 slot="header">{{ mainmsg }}</h1>
      <p slot="subtitle">{{ titlemsg }}</p>
    </my-header>
    <section>
      <div class="box">
        <nuxt-link class="nav_link" to="/">
          <h2>Future World</h2>
        </nuxt-link>
        <p>This web-page to provide one of the sollutions to stop the global warming as well as to decrease the air pollution in the world</p>
        <h3>Description</h3>
        <p>In the main section you will find out a little bit about the global warming</p>
        <p>Next up the website will provide couple of sulutions to solve this problem such as changing your gasoline car to electric or hybrid.</p>
        <p class="main">The site is built and designed to provide information about the current situation with air pollution. APIs are used to provide updated information on electric and hybrid cars for the current day. Electric cars are one of the main solutions to stop the toxic substances being thrown into the atmosphere. Electric, what I believe, is the first step for the bright healthy future for humanity. </p> 
        <p>Designed with the enthusiast in mind</p>
        <h3>Licensing</h3>
        <a href="https://github.com/ymmy1">No Licensing</a>
      </div>
    </section>
  </div>
</template>
<script>
import myHeader from '../components/MyHeader.vue';

export default {
  name: 'about',
  components: {
    myHeader
  },
  data() {
    // returning data
    return {
      mainmsg: 'About Page',
      titlemsg: 'The main idea and purpose of this website'
    }
  },
  head() {
    return {
      meta: [
        { hid: 'description', name: 'description', content: 'Information about the different world we can make together.' }
      ]
    }
  }
}

</script>
<style lang="scss" scoped>
.home {
  background: #fff;
}

.box {
  max-width: 40%;
  min-width: 320px;
  margin: 2% auto 4%;
  background: #eeeeee;
  padding: 2%;
  -webkit-box-shadow: 3px 3px 10px 0px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 3px 3px 10px 0px rgba(0, 0, 0, 0.75);
  box-shadow: 3px 3px 10px 0px rgba(0, 0, 0, 0.75);
}

</style>
