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
	<header>
		<div class="container-fluid text-light">
			<!--navbar-->
			<div class="container-lg p-0">
				<nav class="px-0">
					<ul class="">
						<li>
							<h5 >loremipsum.it</h5>
						</li>
						<li>
							<span class="fw-bold">IT </span> <span>/ EN</span>
						</li>
						<li class="d-none d-md-inline">
							<a href="#">
								<i class="fa-brands fa-twitter"></i>
							</a>
							<a href="#">
								<i class="fa-brands fa-youtube"></i>
							</a>
							<a href="#">
								<i class="fa-brands fa-linkedin"></i>
							</a>
						</li>
					</ul>
				</nav>
			</div>

			<div class="container-sm">
				<div class="row">
					<div class="col-lg-6 col-sm-12">
						<p class="fw-bold">
							Plans are nothing, planning is everything
						</p>
					</div>
					<div class="col-lg-6 col-sm-12">
						<h6 class="text-warning">
							Maria Rossi
						</h6>
						<p>
							Strategic consultant con un focus specifico rivolto a Corporate innovation, buisness growth e Marketing
						</p>

						<a class="p-0" href="#">
							<button class="my-btn">Discover &#8594;</button>
						</a>
					</div>
				</div>
				<div class="d-md-none py-4">
					<a href="#">
						<i class="fa-brands fa-facebook"></i>
					</a>
					<a href="#">
						<i class="fa-brands fa-twitter"></i>
					</a>
					<a href="#">
						<i class="fa-brands fa-youtube"></i>
							</a>
					<a href="#">
						<i class="fa-brands fa-linkedin"></i>
					</a>
				</div>
			</div>
		</div>
	</header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.container-fluid {
	background-image: url(https://s3-alpha-sig.figma.com/img/d7c5/7ec9/4aecaa048b29f54912029661e32e11c2?Expires=1740960000&Key-Pair-Id=APKAQ4GOSFWCW27IBOMQ&Signature=cMpY2SoiSyA~Tg-gIIn~Q79pGd7fNhRc9KcWtXBd9tiRcaz8n9NqO59VJ4jZybRAlYq~zmh9jLOFIGewuKDfol2mhe-lPjIjPX7hSs21gUTtSOkL96JjS0Rr~LCLuyEjBZ0z9tjc2SAYVVVyyru757G91VSF5YkBuV~6~faqQQDNl13OT2Ahx1~A9t6XzmDzVG8PBUb8RA-jmnMJm~utvNDo26V2DQ8st6gbc8jrp6JPQ6VyDcQxPmSy74-ZGvLPkK3jQ-LDw5TYr~iaCxOJyl5cB5NQL7aAjSNAtyTPfVI7Sc-~-e2~uWJmRO-cqgkg7sgUlFDuxbwtncx7JgVT9w__);
	
	background-size: cover;
	
	.container-lg {
		
		nav{
			
			padding: 30px 10px;
			ul {
				list-style: none;
				display: flex;
				justify-content: space-between;
				align-items: center;
				> li {
					cursor: pointer;
					> span:nth-child(2n) {
						opacity: 0.7;
						}
					
				}
				
			}
		}
	}
	.container-sm {
		.row {
			align-items: flex-start;
			padding-bottom: 50px;
			margin-top: 10px;
			.col-lg-6:first-child {
				padding: 50px;
				p {
					font-size: 3.75rem;
					text-align: left;
					line-height: normal;
				}
				
			}
			.col-lg-6:nth-child(2n) {
				padding: 50px;
				h6 {
					margin: 25px 0;
					font-size: 1.25rem;
				}
				p {
					text-align: left;
					margin-bottom: 60px;
					font-size: 1.25rem;
					opacity: 0.8;
				}
				a {
					text-decoration: none;
					.my-btn {
						border: 2px solid white;
						border-radius: 10px;
						background: transparent;
						color: white;
						padding: 5px 15px;
						text-transform: uppercase;
						font-size: 1.1rem;
						
					}
					& :hover {
						border: 2px solid #FCBF49;
						transform: scale(1.1);
						transition: 0.3s;
					}
					
				}
			}
		}
	}
}
a {
	text-decoration: none;
	color: white;
	padding-left: 25px;
	font-size: 1.5rem;
}


@media screen and (max-width: 768px) {
	.container-fluid {
		
		.container-sm {
			.row {
				.col-lg-6:first-child {
					padding: 30px;
					p {
						font-size: 3rem;
					}
				}
				.col-lg-6:nth-child(2n) {
					padding: 30px;
				}
			}
		}
	}
}
</style>
