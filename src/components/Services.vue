<template>
    <h1 class="service">Our Services</h1>
		<div class="container">
			<div class="card">
				<div class="content">
					<h2>01</h2>
					<h3>Web Design</h3>
					<p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Excepturi, beatae?</p>
					<a href="#">Read More</a>
				</div>
			</div>
			<div class="card">
				<div class="content">
					<h2>02</h2>
					<h3>App Design</h3>
					<p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Excepturi, beatae?</p>
					<a href="#">Read More</a>
				</div>
			</div>
			<div class="card">
				<div class="content">
					<h2>03</h2>
					<h3>Graphic Design</h3>
					<p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Excepturi, beatae?</p>
					<a href="#">Read More</a>
				</div>
			</div>
		</div>
</template>
<style scoped> 

.container{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    z-index: 1;
}
.container .card{
    position: relative;
    width: 280px;
    height: 400px;
    margin: 27px;
    box-shadow: 20px 20px 50px rgba(0, 0, 0, 0.5);
    border-radius: 15px;
    background: rgba(255, 255, 255, 0.1);
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    border-top: 1px solid rgba(255, 255, 255, 0.5);
    border-left: 1px solid rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(5px);
}
.container .card .content{
    padding: 20px;
    text-align: center;
    transform: translateY(-100px);
    opacity: 1;
    transition: 0.5s;
}

.container .card .content h2{
    position: absolute;
    top: -80px;
    right: 30px;
    font-size: 8em;
    color:rgba(255, 255, 255, 0.05);
    pointer-events: none;

}
.container .card .content h3{
    font-size: 1.8em;
    color: #000;
    z-index: 1;
}
.container .card .content p{
    font-size: 1em;
    color: #000;
    font-weight: 300;
}
.container .card .content a{
    position: relative;
    display: inline-block;
    margin-top: 16px;
    padding: 8px 20px;
    background: #fff;
    color: #000;
    border-radius: 20px;
    text-decoration: none;
    font-weight: 500;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.2);
}
.service{
    text-align: center;
    font-size: 4em;
    margin:3rem auto;
    color: #000;
}
</style>
