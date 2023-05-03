<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>




<template>
  <header>
   

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

header {
 background: #D9CFDE;
 position: fixed; /* vai fixiar a posição, mesmo se scrola vai ficar no msm lugar*/
 top: 0;
 z-index: 2 ; /* para trazer o header mais pra frente, pq o main estava em cima dele*/
 width: 100vw; /* a largura vai ficar do tamanho da tela (vw - view port) */

 display: flex; /* trabalhar com tamanhos flexives  (bianca ficou grande e home about ficou na msm linha so q menorzinho*/
 /* justify-content: center ;   mexer nos elementos da linha*/
 justify-content: space-between; /* vai separar os elementos no estremo */
 padding: 2rem; /* da o espaçamento q vc quer */ 
 align-items: center; /*  vai alinhar os elementos da linha*/
 height: 10vh;
}



header nav{
  display: flex;
  justify-content: space-between;
  min-width: 30%;
}


main {
  padding-top: 10vh ;
 background: green;
 min-height: 120vh; /* tamanho do meio da pg  */
 
}

footer {
  background: red;
}



</style>

<!-- 
  
  header nav {} -> estiliza o nav

  headar #titulo -> vai estilizar td os #titulos q estejam no header

  #titulo -> vai estilizar todos os #titulos
  
  # seletor de elemento que tenha um id  (#link-mais-legal)

. seletor de classe (.elemento-mais-legal) 

* { } -> seleciona tudo tudo  

header button.primary interroga


-->

<!-- ESTAVA DENTRO DO STYLO ORIGINAL de cima, PROF APAGOU
    @keyframes trinity-rings-spinner-circle1-animation{
      0% {
        transform: rotateZ(20deg) rotateY(0deg);
      }
      100% {
        transform: rotateZ(100deg) rotateY(360deg);
      }
    }
    @keyframes trinity-rings-spinner-circle2-animation{
      0% {
        transform: rotateZ(100deg) rotateX(0deg);
      }
      100% {
        transform: rotateZ(0deg) rotateX(360deg);
      }
    }
    @keyframes trinity-rings-spinner-circle3-animation{
      0% {
        transform: rotateZ(100deg) rotateX(-360deg);
      }
      100% {
        transform: rotateZ(-360deg) rotateX(360deg);
      }
    }


header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
} 
 -->
