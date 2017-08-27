<template>
  <div id="app">

    <layout></layout>

    <header class="m-header">
      <div class="m-header__logo">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 243.58 57.85">
          <path d="M49.65 17.63v22.59h17.63v-3.96H53.89v-5.65h9.33v-3.95h-9.33v-5.07h13.39v-3.96H49.65m28.62 16.04a9.51 9.51 0 0 0 6.8 3.06c3.22 0 5.49-1.22 5.49-3.38 0-5-14.81-.18-14.81-9.39 0-4 4.28-6.8 9.51-6.8a12.43 12.43 0 0 1 9.14 3.45l-3.15 2.77A8.35 8.35 0 0 0 85 20.69c-3.51 0-4.83 1.69-4.83 3.06 0 5.07 14.81 0 14.81 9.39 0 4.71-4.86 7.55-10.13 7.55a13.72 13.72 0 0 1-9.84-4.17zM125 36a12.39 12.39 0 0 1-9.8 4.64c-6.88 0-12.33-5.14-12.33-11.76s5.45-11.76 12.33-11.76a12.39 12.39 0 0 1 9.8 4.68l-3.51 2.59a7.51 7.51 0 0 0-6.29-3.27 7.81 7.81 0 1 0 6.36 12.48zm38.31-18.37h4.24v22.59h-4.24zm28 0l-5.59 13.81-5.6-13.81h-4.57l10.17 23.06 10.17-23.06h-4.58m22.31 19.1a7.81 7.81 0 1 0-7.86-7.81 7.92 7.92 0 0 0 7.86 7.81m0-19.57c6.88 0 12.32 5.14 12.32 11.76s-5.45 11.76-12.32 11.76-12.32-5.14-12.32-11.76 5.45-11.76 12.33-11.76m-74.87 11.98h6.36c3 0 4.35-1.76 4.35-3.78s-1.35-3.78-4.35-3.78h-6.36zm-4.24-11.51h10.94c5.12 0 8.26 3.31 8.26 7.74a7.21 7.21 0 0 1-5.38 6.8l5.74 8.06h-5.34L144 33.1h-5.19v7.12h-4.24z" />
          <path fill="#fc4b1f" d="M17.63 26.66h16.31v3.96H17.63zm2.74-9.03H38v3.96H20.37zm0 18.63H38v3.96H20.37z" />
        </svg>
      </div>
      <div class="m-header__tagline">
        <h2 class="m-header__tagline__title">{{ tagline }}        
          <button title="Add a new entry" class="button--round">+</button></h2>
      </div>
    </header>
    <card></card>
  </div>
</template>

<script>
import Layout from './components/Layout.vue'
import card from './components/Card.vue'
export default {
  name: 'app',
  components: { Layout, card },
  data() {
    return {
      tagline: 'Our quarterly priorities to October 2017'
    }
  }
}
</script>

<style scoped>

.m-header {
  display: grid;
  grid-template-areas: "m-header__logo m-header__tagline";
  grid-template-columns: [m-header__logo-start] 1fr [m-header__logo-end] 
  [m-header__tagline-start] 2fr [m-header__tagline-end];
  grid-auto-rows: auto;
}


.m-header__logo {
  // grid-column-start: 1;
  // grid-column-end: 2;
  // grid-column: 1/2;
  grid-area: m-header__logo;
  grid-column: [m-header__logo-start] / [m-header__logo-end] ;
  height: auto;
  padding: 1rem;
  min-width: 170px;
  max-width: 500px;
}



.m-header__tagline {
  // grid-column-start: 3;
  // grid-column-end: 4;
  grid-column: 3/4;
  padding: 1rem;
}

.m-header__tagline__title {
     font-size: calc(80% + 1vw); 
}

.button--round {
  font-size: 25px; 
  height: 30px;
  width: 30px;
  margin-left: 1rem;
  background-color: white;
  color: #EA7E3D;
  border-radius: 50%;
  border: 1px solid var(--color-orange);
  transition: all 0.3s cubic-bezier(.25, .8, .25, 1);
}

.button--round:hover {
  background-color: var(--color-orange);
  color: white;
  border: 1px solid var(--color-white);
}

#app {}
</style>
