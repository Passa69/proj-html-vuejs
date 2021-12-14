<template>
  <div id="app">
    <header>
      <MyHeader/>
    </header>

    <div>
      <MyMain/>

      <MyFooter :links1="footLinksAdd" :links2="footLinksEx" :links3="footLinks" :links4="footLinksInfo"/>
    </div>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  },
  data() {
    return {
      footLinksAdd: [
        {
          title: "Address",
          coordinates: "382 NE 191st St # 87394 Miami, FL 33179-3899",
          timetables: "+1 (305) 547-9909 (9am-5pm EST, Monday-Friday)",
          mail: "support@maxcoach.com"
        }
      ],

      footLinksEx: [
        {
          title: "Explore",
          start: "Start here",
          blog: "Blog",
          info: "About us"
        }
      ],

      footLinks: [
        {
          story: "Success story",
          culture: "Courses",
          contact: "Contact us"
        }
      ],

      footLinksInfo: [
        {
            title: "Information",
            member: "Membership",
            guide: "Purchase guide",
            police: "Pricavy police",
            service: "Terms of service"
        }
      ],
    }
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

  header {
    background-color: #e9e6e3;
  }

  div {
    width: 80%;
    margin: 0 auto;
  }
}
</style>
