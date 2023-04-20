<template>
     <div> 
    <div class="flex items-center p-3 mt-2 dark:bg-gray-900">
          <div
            class="flex-1 max-w-md mx-auto overflow-hidden bg-white rounded-lg shadow-xl h-70 dark:bg-gray-800"
          >
            <form class="flex flex-col overflow-y-auto ">
     
              <div class="flex items-center justify-center p-6 sm:p-12 md:w-md">
                <div class="w-full">
                  <h1
                    class="mb-4 text-xl font-semibold text-center text-gray-700 dark:text-gray-200" 
                  >
                    Registration
                     </h1>
               
                      <label class="block text-sm">
                            <span class="text-gray-700 dark:text-gray-400">Username</span>
                            <input
                              class="block w-full mt-1 text-sm dark:bg-gray-700 focus:outline-none dark:text-gray-300 form-input" name="username"
                              placeholder="Veillez saisir votre prenom" 
                            />
                          </label>
                       <label class="block text-sm">
                        <span class="text-gray-700 dark:text-gray-400">Email</span>
                        <input
                          class="block w-full mt-1 text-sm dark:bg-gray-700 focus:outline-none dark:text-gray-300 form-input" name="email"
                          placeholder="Veillez saisir votre email" 
                        />
                      </label>
                      <label class="block mt-4 text-sm">
                        <span class="text-gray-700 dark:text-gray-400">Password</span>
                        <input
                          class="block w-full mt-1 text-sm dark:bg-gray-700 focus:outline-none dark:text-gray-300 form-input"
                          placeholder="Veillez saisir votre mot de passe" name="password"
                          type="password" 
                        />
                      </label>

                     <div class="flex mt-6 text-sm">
                    <label class="flex items-center dark:text-gray-400">
                      <input
                        type="checkbox"
                        class="text-blue-400 form-checkbox focus:border-blue-400 focus:outline-none focus:shadow-outline-blue-400 dark:focus:shadow-outline-gray"
                      />
                      <span class="ml-2">
                        I agree to the
                        <span class="underline">privacy policy</span>
                      </span>
                    </label>
                  </div>

            
                  <button
                    class="block w-full px-4 py-2 mt-4 text-sm font-medium leading-5 text-center text-white transition-colors duration-150 bg-blue-400 border border-transparent rounded-lg active:bg-blue-400 hover:bg-blue-300 focus:outline-none focus:shadow-outline-purple"
                    type="submit"
                  >
                    Create account
                  </button>
            
                </div>
              </div>
            </form>
          </div>
          </div>
          </div>
   
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Register',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
