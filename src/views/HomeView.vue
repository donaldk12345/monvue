<!-- eslint-disable no-mixed-spaces-and-tabs -->
<!-- eslint-disable no-mixed-spaces-and-tabs -->
<template>
    <div class="bg-fixed w-full" style="background-image: linear-gradient(rgba(57, 49, 49, 0.618),rgba(57, 49, 49, 0.618)),url(images/php.jpg);height: 70vh; background-position: center center; background-size: cover; background-repeat: no-repeat;">
      <div class="m-auto flex max-w-sm flex-col items-center pt-3"><br><br><br>
         <h3 class="max-w-2xl text-center text-3xl font-bold leading-tight md:text-3xl sm:text-2xl md:leading-tight text-neutral-100">Bienvenue sur Ynodev</h3>
          <p class="mt-3 text-center  text-neutral-300 text-sm">Votre service de digitalisation et réalisation de vos projets dans le domaine des TIC</p>
     

      </div>
    </div>
   <div className="w-full bg-white py-16 px-4 mt-2">
              <div className=" max-x-w-[1240px]  gap-2 grid md:grid-cols-2 sm:grid-cols-1 lg:grid-cols-2">
                  <img class="w-[350px] mx-auto my-auto" src="images/dev.jpg" alt="" />

           
                <div class=" justify-center text-center px-2 mt-2 m-auto">
                  <p class="font-bold text-blue-300">Nous connaitte</p>
                  <h1 class="md:text-3xl sm:text-1xl font-bold py-2  text-gray-500 dark:text-gray-400">C'est quoi Ynodev ?</h1>
                  <p class="text-center  font-mono text-gray-500 dark:text-gray-400 text-sm">
                      Ynodev est une  plateforme créer pour répondre au bésoin des entreprise  dans le domaine des TIC notament en développement 
                      d'applications , maintenance informatique et réseaux .
                      </p>
                      <button className=" bg-blue-300 active:bg-blue-400 hover:bg-blue-400 focus:outline-none w-[200px] rounded-md  font-medium p-2 mx-auto   text-white my-2 justify-center m-auto text-center " >Sourmettre un projet</button>

                  </div>
               </div>
          
             
          </div>


    <div class="w-full  bg-primary-light px-20 py-14">
      <div class="mx-auto flex max-w-sm flex-col items-center">
        <h3 class="max-w-2xl text-center text-2xl font-bold leading-tight sm:text-3xl md:text-2xl md:leading-tight">S'abonner</h3>
        <p class="mt-3 text-center  text-gray-500 dark:text-gray-400 text-sm">Abonnez vous à notre news letter afin de bénéficier des meilleurs offres et astuces</p>
        <form action="" class="mx-auto mt-6 flex w-full flex-col gap-1 px-2 sm:flex-row">
            <input class="block w-full mt-1 text-sm  dark:bg-gray-700 focus:outline-none  dark:text-gray-300  form-input" name="email"   v-model="email"
                        placeholder="Veillez saisir votre adresse mail" 
                      />
          <button type="submit" class="rounded-lg bg-stone-900 px-3 py-3 font-bold text-white">Envoyer</button>
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
