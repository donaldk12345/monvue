<!-- eslint-disable vue/multi-word-component-names -->
// eslint-disable-next-line vue/multi-word-component-names
<template>
    <div class=" shadow-sm text-[#505352] bg-white rounded-lg">
        <nav class="container px-6 py-5 mx-auto md:flex md:justify-between md:items-center">
            <div class="flex items-center justify-between">
                <router-link to="/" class="w-full text-2xl font-bold text-blue-300 md:text-2xl hover:text-blue-400">Ynodev
                </router-link>
                <!-- Mobile menu button -->
                <div @click="toggleNav" class="flex md:hidden">
                    <button type="button" class="text-blue-300 hover:text-gray-400 focus:outline-none focus:text-gray-400">
                        <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                            <path fill-rule="evenodd"
                                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z">
                            </path>
                        </svg>
                    </button>
                </div>
            </div>

            <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
            <ul :class="showMenu ? 'flex' : 'hidden'" class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
                <li class="text-[#505352] hover:text-blue-400">Home</li>
                <li class="text-[#505352] hover:text-blue-400">About</li>
                <li class="text-[#505352] hover:text-blue-400" ><router-link to="/login">Se connecter</router-link> </li>
                <li class="text-[#505352] hover:text-blue-400"> <router-link to="/register">Apropos</router-link> </li>
            </ul>
        </nav>
    </div>
</template>
<script>
import { ref } from 'vue';
export default {
    setup() {
        let showMenu = ref(false);
        const toggleNav = () => (showMenu.value = !showMenu.value);
        return { showMenu, toggleNav };
    },
};
</script>