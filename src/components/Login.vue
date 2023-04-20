<!-- eslint-disable vue/multi-word-component-names -->
<template>
      <div>           
        <div className="flex items-center  mt-5 p-3 dark:bg-gray-900">
          <div
            className="flex-1 h-70 max-w-md mx-auto overflow-hidden bg-white rounded-lg shadow-xl dark:bg-gray-800"
          >
            <div className="flex flex-col overflow-y-auto ">
     
                  <div className="flex items-center justify-center p-6 sm:p-12 md:w-md">
                  <form  className="w-full"  @submit.prevent="handleSubmit">
                   <div className="w-full">
                  <h1
                    className="mb-4 text-xl font-semibold text-gray-700 dark:text-gray-200 text-center" 
                  >
                    Login
                  </h1>
                  <label className="block text-sm">
                    <span className="text-gray-700 dark:text-gray-400">Email</span>
                    <input
                      className="block w-full mt-1 text-sm  dark:bg-gray-700 focus:outline-none  dark:text-gray-300  form-input" name="email"   v-model="email"
                      placeholder="Veillez saisir votre nom" 
                    />
                  </label>
                  <label className="block mt-4 text-sm">
                    <span className="text-gray-700 dark:text-gray-400">Password</span>
                    <input
                      className="block w-full mt-1 text-sm  dark:bg-gray-700  focus:outline-none  dark:text-gray-300  form-input"   v-model="password"
                      placeholder="Veillez saisir votre mot de passe" name="password"
                      type="password" 
                    />
                  </label>

              
                  <button
                    className="block w-full px-4 py-2 mt-4 text-sm font-medium leading-5 text-center text-white transition-colors duration-150 bg-blue-400 border border-transparent rounded-lg active:bg-blue-400 hover:bg-blue-300 focus:outline-none focus:shadow-outline-purple" type="submit"
              
                  >
                    Connexion
                  </button>

                  <p className="mt-4">
                    <a
                      className="text-sm font-medium text-blue-400 dark:text-blue-400 hover:underline"
                      href="./forgot-password.html"
                    >
                      Forgot your password?
                    </a>
                  </p>
                  <p className="mt-1">
                    <a
                      className="text-sm font-medium text-blue-400 dark:text-blue-400 hover:underline"
                      href="./create-account.html"
                    >
                     <router-link to="/register">Créer un compte</router-link>
                    </a>
                  </p>
                    </div>
                    </form>
              </div>
            </div>
          </div>
          </div>
            </div>
</template>

<script>
import axios from 'axios';
// eslint-disable-next-line no-unused-vars

export default {
    // eslint-disable-next-line vue/multi-word-component-names
  name: 'Login',
  // props: ['user'],
  data() {
    return {
      email: '',
      password: '',
      //user: null,
      error: '',
      success: ''
    }
  },
     methods: {


    handleSubmit() {
      this.error = '';
      this.success = '';
      axios.post('http://localhost:3000/api/login', {
        email: this.email,
        password: this.password
      }
      ).then(response => {
        console.log(response);
        //const t= data.token
        // sessionStorage.setItem('user', JSON.stringify(response.data));
        this.$router.push('/');
        
        // window.location.reload();

      }).catch(error => {
        if (error) {
          console.log(error)
          //this.error = error.response.data.message;
          //this.error = 'Le mot de passe ou l\'email saisir est incorrect !';

        } 

      })








    }

  }
 
}
</script>

<style></style>
