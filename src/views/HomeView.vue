<!-- eslint-disable no-mixed-spaces-and-tabs -->
<!-- eslint-disable no-mixed-spaces-and-tabs -->
<template>
    <div class="w-full bg-fixed" style="background-image: linear-gradient(rgba(57, 49, 49, 0.618),rgba(57, 49, 49, 0.618)),url(images/php.jpg);height: 70vh; background-position: center center; background-size: cover; background-repeat: no-repeat;">
      <div class="flex flex-col items-center max-w-sm pt-3 m-auto"><br><br><br>
         <h3 class="max-w-2xl text-3xl font-bold leading-tight text-center md:text-3xl sm:text-2xl md:leading-tight text-neutral-100">Bienvenue sur Ynodev</h3>
          <p class="mt-3 text-sm text-center text-neutral-300">Votre service de digitalisation et réalisation de vos projets dans le domaine des TIC</p>
     

      </div>
    </div>
   <div className="w-full bg-white py-16 px-4 mt-2">
              <div className=" max-x-w-[1240px]  gap-2 grid md:grid-cols-2 sm:grid-cols-1 lg:grid-cols-2">
                  <img class="w-[350px] mx-auto my-auto" src="images/dev.jpg" alt="" />

           
                <div class="justify-center px-2 m-auto mt-2 text-center ">
                  <p class="font-bold text-blue-300">Nous connaitte</p>
                  <h1 class="py-2 font-bold text-gray-500 md:text-3xl sm:text-1xl dark:text-gray-400">C'est quoi Ynodev ?</h1>
                  <p class="font-mono text-sm text-center text-gray-500 dark:text-gray-400">
                      Ynodev est une  plateforme créer pour répondre au bésoin des entreprise  dans le domaine des TIC notament en développement 
                      d'applications , maintenance informatique et réseaux .
                      </p>
                      <button className=" bg-blue-300 active:bg-blue-400 hover:bg-blue-400 focus:outline-none w-[200px] rounded-md  font-medium p-2 mx-auto   text-white my-2 justify-center m-auto text-center " >Sourmettre un projet</button>

                  </div>
               </div>
          
             
          </div>


    <div class="w-full px-20 bg-primary-light py-14">
      <div class="flex flex-col items-center max-w-sm mx-auto">
        <h3 class="max-w-2xl text-2xl font-bold leading-tight text-center sm:text-3xl md:text-2xl md:leading-tight">S'abonner</h3>
        <p class="mt-3 text-sm text-center text-gray-500 dark:text-gray-400">Abonnez vous à notre news letter afin de bénéficier des meilleurs offres et astuces de Ynodev</p>
        <form action="" class="flex flex-col w-full gap-1 px-2 mx-auto mt-6 sm:flex-row">
            <input class="block w-full mt-1 text-sm dark:bg-gray-700 focus:outline-none dark:text-gray-300 form-input" name="email"   v-model="email"
                        placeholder="Veillez saisir votre adresse mail" 
                      />
          <button type="submit" class="px-3 py-3 font-bold text-white rounded-lg bg-stone-900">Envoyer</button>
        </form>
      </div>
    </div>
 
     
</template>
<script>
export default {
  name: 'HomeView',

  methods: {
   
  }

};
</script>
