<script>
import { store } from '../store.js';
export default {
  data() {
    return { 
      
    }
  }
}
</script>

<template>
	<section>
		<div class="container-sm">
			<h3>
				Biography
			</h3>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur numquam dignissimos quae animi provident veritatis quas itaque rem earum quasi minima ducimus praesentium recusandae maiores eligendi illum, non reiciendis rerum eos? Magnam dolor sed deserunt veritatis, nostrum est odio facere ipsam, iusto et sit non provident consequuntur quas? Iste aliquam ad sunt, quaerat cum debitis inventore, mollitia aperiam tempora suscipit tenetur maxime adipisci? Aut adipisci quam sint repellendus nesciunt molestias doloremque optio sequi temporibus, aliquid dicta quo alias deleniti corrupti atque provident voluptates dolor doloribus error ab sit tempora! Molestias perspiciatis saepe est rem, ducimus quaerat optio necessitatibus placeat magnam.
			</p>
			<a href="#">
				<button class="my-btn">Read more</button>
			</a>
			<h3 class="pt-5">
				Expertise
			</h3>
		</div>
	</section>
	
	
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


	section {
		background-color: black;
		text-align: center;
		padding: 50px;
		
		.container-sm {
			padding: 0px 250px ;
			color: white;
			opacity: 0.9;
			h3 {
				margin: 40px 0;
				text-transform: uppercase;
				font-size: 1.5rem;
			}
			p {
				padding: 10px 100px;
				text-align: left;
				font-size: 0.8rem;
			}
			a {
				text-decoration: none;
					.my-btn {
						border: 2px solid white;
						border-radius: 10px;
						background: transparent;
						color: white;
						padding: 5px 20px;
						text-transform: uppercase;
						
					}
				& :hover {
					border: 2px solid #FCBF49;
				}
					
			}
		}
	}





</style>