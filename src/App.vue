<!-- eslint-disable no-undef -->
<template>
  <Nav />
  <router-view/>
  <Footer />
</template>
<script>
import Nav from './components/Nav.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',

  data() {

    
    return {
      currentUser: '',
      user: null
    }

  },
  methods: {
    
  },
  created() {

     this.currentUser = JSON.parse(sessionStorage.getItem('user'));
    console.log('mon user', this.currentUser);

    // // eslint-disable-next-line no-unused-vars
    // const token = window.localStorage.getItem('jwt');

    // axios.get('http://localhost:8000/api/user', {

    //   headers: {
    //     'Content-Type': 'application/json',
    //     Authorization: `Bearer ${token}`
    //   }


    // }

    // ).then((response) => {

    //   this.user = response.data;
    //   console.log(this.user);

    // });
  },
  components: {
    Nav,
    Footer

  }

}
</script>

<style>

</style>
