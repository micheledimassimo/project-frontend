<script>
import { store } from '../store.js';
export default {
  data() {
    return { 
      clients: [
        "Laurene", "-", "wood", "-", "italia", "-", "rik", "-", "eco", "-",
        "vogue", "-", "klee", "-", "kless", "-", "rita", "-", "Laurene", "-",
        "wood", "-", "italia", "Laurene", "-", "wood", "-", "italia", "-", "rik", "-", "eco", "-",
        "vogue", "-", "klee", "-", "kless", "-", "rita", "-", "Laurene", "-",
        "wood", "-", "italia", "Laurene", "-"
      ]
    }
  }
}
</script>

<template>
	<footer>
    <div class="py-5">
      <h3 class="text-center text-light py-5 text-uppercase">
      Clients & collaboratores
      </h3>
      <!--slider-->
      <div class="slider">
          <div class="slide-track">
            <div class="slide" v-for="(name, index) in clients" :key="index">
              <span class="ms-3 text-uppercase">{{ name }}</span>
            </div>
          </div>
      </div>
    </div>
    <div class="py-5 d-none d-lg-block">
      <div class="row text-white text-center justify-content-around ">
        <div class="col-4">
          <a href="#">
            loremipsum.com
          </a>
        </div>
        <div class="col-4 custom-opacity">
          <span>
            E-mail: info@example.com
          </span>
        </div>
        <div class="col-4 custom-opacity">
          <span class="me-4">
            twitter
          </span>
          <span class="ms-4">
            linkedin
          </span>
        </div>
      </div>
    </div>

    <!--link footer mobile-->
    <div class="text-center d-lg-none">
      <div>
        <a href="#">
          loremipsum.com
        </a>
      </div>
      <div>
        <hr>
      </div>
      <div class="py-4">
        <span class="text-light custom-opacity  ">
          E-mail: info@example.com
        </span>
      </div>
      <div>
        <a href="#">
						<i class="fa-brands fa-facebook"></i>
					</a>
					<a href="#">
						<i class="fa-brands fa-twitter"></i>
					</a>
					<a href="#">
						<i class="fa-brands fa-linkedin"></i>
					</a>
      </div>

    </div>

    <div id="pièpag" class="text-center text-secondary pt-4">
      
        © 2021 Tutti i diritti riservati - Design by MM
      
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

footer {
  background-color: #010d10;
  .slider {
    border: 1px solid #FCBF49;
    border-left: none;
    border-right: none;
    overflow: hidden;
    white-space: nowrap;
    position: relative;
  }

  .slide-track {
    display: flex;
    width: 100%; /* Doppia larghezza per il loop continuo */
    animation: slide-left 8s linear infinite;
  }

  .slide {
    flex: none;
    font-size: 1.5rem;
    color: #FCBF49;
    padding: 0 10px;
  }

  @keyframes slide-left {
    from {
      transform: translateX(0);
    }
    to {
      transform: translateX(-100%); 
    }
  }

  a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    > i {
      padding: 30px 20px;
      font-size: 1.5rem;
    }
  }
  .custom-opacity {
    opacity: 0.85;
  }

  hr {
    font-size: 5px;
    width: 80%;
    color: white;
    margin: 20px auto 0;
  }

  #pièpag {
    font-size: 0.75rem;
    opacity: 0.8;
    padding-bottom: 10px;
  }
}



</style>
