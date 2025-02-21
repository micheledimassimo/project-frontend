<script>
import { store } from '../store.js';
export default {
  data() {
    return { 
      isHidden : false
    }
  },
  methods: {
	changeHidden() {
		if (!this.isHidden) {
			this.isHidden = true
			return this.isHidden
		}
		if (this.isHidden) {
			this.isHidden = false
			return this.isHidden
		}
	}
  }
}
</script>

<template>
	<section>
		<div v-show="!isHidden" class="container-sm ">
			<h3>
				Biography
			</h3>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur numquam dignissimos quae animi provident veritatis quas itaque rem earum quasi minima ducimus praesentium recusandae maiores eligendi illum, non reiciendis rerum eos? Magnam dolor sed deserunt veritatis, nostrum est odio facere ipsam, iusto et sit non provident consequuntur quas? Iste aliquam ad sunt, quaerat cum debitis inventore, mollitia aperiam tempora suscipit tenetur maxime adipisci? Aut adipisci quam sint repellendus nesciunt molestias doloremque optio sequi temporibus, aliquid dicta quo alias deleniti corrupti atque provident voluptates dolor doloribus error ab sit tempora! Molestias perspiciatis saepe est rem, ducimus quaerat optio necessitatibus placeat magnam.
			</p>
			
			<button @click="changeHidden" class="my-btn">Read more</button>
			
			
		</div>
		<!--blocco inizialmente non visibile-->
		<div v-show="isHidden" class="row container-sm ">
			<h3>
				Biography
			</h3>
			<div class="col-lg-6 col-sm-12">
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam voluptas similique voluptates excepturi quo a rerum facere, earum unde inventore necessitatibus, quaerat fugit, at quam ipsam molestias consequatur pariatur ab? Enim reprehenderit incidunt officiis soluta, fugiat ab adipisci laudantium delectus, voluptate ea consectetur earum similique expedita itaque saepe? Delectus excepturi libero minus dolorum, perspiciatis quia sint explicabo odio. Quia quibusdam earum numquam assumenda laboriosam consequatur quam doloremque vitae, molestias laborum blanditiis beatae fuga saepe laudantium illum iure minima eos accusantium harum. Totam tempore tenetur, quas consequatur delectus possimus non quaerat ad ex minima maiores atque vitae, corrupti nam perferendis? Aut.
				</p>
			</div>
			<div class="col-lg-6 col-sm-12">
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa eius consequuntur asperiores obcaecati eaque, ipsa dicta! Aliquid veritatis fugit beatae sequi, amet nam modi optio culpa placeat quas nobis ut ex unde totam dicta sed praesentium facere nisi dolorem iste earum, assumenda quaerat molestiae! Impedit id eligendi placeat illum debitis expedita iure praesentium doloremque repellat vitae, quos maiores beatae autem dolore incidunt libero aliquid voluptates cumque ratione quia nam! Deleniti similique consequuntur pariatur quia quam repellendus animi officiis nulla cupiditate corporis dolores, non nemo, vitae optio nostrum! At fugit quidem, excepturi asperiores neque illo expedita, explicabo quos nulla voluptatibus perspiciatis.
				</p>
				
				<button @click="changeHidden" class="my-btn">less</button>
				
			</div>
		</div>
		
	</section>
	
	
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


	section {
		background-color: black;
		text-align: center;
		padding: 50px;
		
		.container-sm:first-child {
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
			
			.my-btn {
				border: 2px solid white;
				border-radius: 10px;
				background: transparent;
				color: white;
				padding: 5px 20px;
				text-transform: uppercase;
				
				}
				.my-btn:hover {
					border: 2px solid #FCBF49;
					transform: scale(1.1);
					transition: 0.3s;
					}
				
					
			}
		}
		.container-sm:nth-child(2n) {
			color: white;
			margin: 50px auto;
			padding: 0px 250px;
			position: relative;
			h3 {
				margin: 40px 0;
				text-transform: uppercase;
				font-size: 1.5rem;
			}
			p {
				text-align: left;
				font-size: 0.9rem;
				margin-bottom: 20px;
			}
			
			.my-btn {
				border: 2px solid white;
				border-radius: 10px;
				background: transparent;
				color: white;
				padding: 5px 10px;
				text-transform: uppercase;
				position: absolute;
				top: 100%;
				right: 12%;	
				
			}
			.my-btn:hover {
				border: 2px solid #FCBF49;
				transform: scale(1.1);
				transition: 0.3s;
			}
				
		}
		
@media screen and (max-width: 768px) {
	section {
		.container-sm:first-child {
			padding: 0px;
			p {
				padding: 10px 10px;
				text-align: left;
				font-size: 0.8rem;
			}
		}

		.container-sm:nth-child(2n) {
			padding: 0px;
			p {
				padding: 10px 10px;
				text-align: left;
				font-size: 0.8rem;
			}
		}
	}
}



</style>