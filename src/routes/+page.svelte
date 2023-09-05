<script>
	import { quintOut } from "svelte/easing";
	import { fade, draw, fly } from "svelte/transition";
	import { expand } from "../custom-transitions.js";
	import { inner, outer } from "../shape.js";

	import "../app.css";


	let visible = true;
</script>
<!-- 
{#if visible}
	<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 103 124">
		<g out:fade="{{duration: 200}}" opacity=0.2>
			<path
				in:expand="{{duration: 400, delay: 1000, easing: quintOut}}"
				style="stroke: #ff3e00; fill: #ff3e00; stroke-width: 50;"
				d={outer}
			/>
			<path
				in:draw="{{duration: 1000}}"
				style="stroke:#ff3e00; stroke-width: 1.5"
				d={inner}
			/>
		</g>
	</svg>

	<div class="centered" out:fly="{{y: -20, duration: 800}}">
		{#each 'SVELTE' as char, i}
			<span
				in:fade="{{delay: 1000 + i * 150, duration: 800}}"
			>{char}</span>
		{/each}
	</div>
{/if} -->

<div class="right-align">
	<img src="../logo_dark_cropped.png" alt="logo" width="40%" height="40%" class="logo" > 

</div>


<div class="container mx-auto flex px-10 py-20 md:flex-row flex-col items-center">

<div id="outer" class="text-box">
	<h1 id="inner" class="sm:text-8xl text-dark title spaced-letters">
		Simplify your streaming 
		 <!-- {/* <br class="hidden lg:inline-block" />I love to build amazing
		 apps. */} -->
	   </h1>
	  <br>
	  <br>
	<button class="bg-white hover:bg-purple-700 font-semibold text-gray-800 py-2 px-4 rounded buttons">
		Log In
	</button>
	<br>
	<br>
	<button class="bg-pink-600 hover:bg-purple-700 font-bold py-2 px-4 rounded buttons">
		Sign Up
	</button>
	<br>
	<br>
</div>



<div class="right-align">




</div>	
</div>


<!-- <div class="container mx-auto flex px-10 py-20 md:flex-row flex-col items-center"> -->
	  <!-- <div class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center"> -->
	
		<!-- <p class="mb-8 leading-relaxed">
		  I code to solve problems.
		</p>
		<div class="flex justify-center">
		  <a
			href="#contact"
			class="inline-flex text-white bg-purple-800 border-0 py-2 px-6 focus:outline-none hover:bg-green-900 rounded text-lg">
			Work With Me
		  </a>
		  <a
			href="#projects"
			class="ml-4 inline-flex text-gray-200 bg-gray-800 border-0 py-2 px-6 focus:outline-none hover:bg-gray-700 hover:text-white rounded text-lg">
			See My Work
		  </a>
		</div>
	  </div> -->
		<!-- {/* <img
		  class="object-cover object-center rounded"
		  alt="hero"
		  src="./coding.svg"
		/> */} -->
	<!-- </div> -->
<!-- </div> -->


<link href="https://fonts.googleapis.com/css?family=Overpass:100,400" rel="stylesheet">



<style>

	.logo {
		padding-top: 2rem;
	}

	.spaced-letters {
		letter-spacing: 1rem;
		color:blanchedalmond;

	}


	.right-align {
		padding-left: 91%;
	}

	.buttons {
		width: 25%;
		/* color: #ffebcd; */
	}

	/* svg {
		width: 100%;
		height: 10%;
	}

	path {
		fill: white;
		opacity: 1;
	} */

	#inner {
		display: table;
		margin: 0 auto;
		padding-top: 5%;

		/* border: 1px solid black; */
	}

	#outer {
	/* border: 1px solid red; */
	width:100%;
	width: 100%;
	height: 100%;
    background-image:url('../bg_1.png') no-repeat center center fixed;

	}

	.title {
		padding-top: 200px;
	}

	/* html {
		height: 100%;
	}
	body {
		min-height: 100%;
	}

	body.home {
		background: url(/wp-content/uploads/2015/03/achtergrond2.jpg) no-repeat center center fixed;
		background-size: cover;
	} */



    :global(body){
        background-color: lightseagreen;
        background-image: url("https://images.pexels.com/photos/956981/milky-way-starry-sky-night-sky-star-956981.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260");
        background: url("../bg_shifted.png") no-repeat center center fixed;
	    /* background:url('../bg_1.png') no-repeat center center fixed; */
    	background-size:cover;
    }

    :global(body.dark-mode) {
        background-color: #1d3040;
        color: #bfc2c7;
    }

	/* .center-div {
		margin: auto;
	}

	.custom-label {
		position: relative;
		justify-content: center;
		align-items:stretch;

	}

	label {
		position: absolute;
		top: 1em;
		left: 1em;
	}  */

	/*
	.centered {
		font-size: 20vw;
		position: absolute;
		left: 50%;
		top: 50%;
		transform: translate(-50%,-50%);
		font-family: 'Overpass';
		letter-spacing: 0.12em;
		color: #676778;
		font-weight: 400;
	}

	.centered span {
		will-change: filter;
	}  */

</style>