<template>
  <div class="flex flex-col justify-items-center content-center items-center">
    <transition appear 
      appear-class="top-appear-class"
			appear-to-class="top-appear-to-class"
			appear-active-class="top-appear-active-class">
      <img class="profile rounded-full border-solid border-2 border-blue-400 shadow-lg" src="./profile.jpg"/>
      </transition>
     <transition appear 
      appear-class="bottom-appear-class"
			appear-to-class="bottom-appear-to-class"
			appear-active-class="bottom-appear-active-class">  
      <h1 class="tracking-wide text-3xl mt-8">Felicidades <span class="text-blue-400">Papá</span></h1>
    </transition>
    <transition appear 
      appear-class="bottom-appear-class"
			appear-to-class="bottom-appear-to-class"
			appear-active-class="bottom-appear-active-class">
      <p class="font-serif mt-10 ml-12 mb-20 mr-12">Por muchos más días de los padres juntos, sigue viendo:</p>
    </transition>
    <h3 class="font-serif">Por más momentos en familia</h3>
 <transition appear 
      appear-class="left-appear-class"
			appear-to-class="left-appear-to-class"
			appear-active-class="left-appear-active-class">
      <img class="image ml-10 mr-10 mt-3 rounded shadow-xl" src="./pic1.jpg"/>
      </transition>
         <h3 class="font-serif mt-5 ">Por un hotel cuando mejore la economía jaja</h3>
 <transition appear 
      appear-class="left-appear-class"
			appear-to-class="left-appear-to-class"
			appear-active-class="left-appear-active-class">
      <img class="image ml-10 mr-10 mt-3 rounded shadow-xl" src="./pic2.jpg"/>
      </transition>
   <h3 class="font-serif mt-5 ">Por una Puti siempre feliz</h3>
 <transition appear 
      appear-class="left-appear-class"
			appear-to-class="left-appear-to-class"
			appear-active-class="left-appear-active-class">
      <img class="image ml-10 mr-10 mt-3 rounded shadow-xl" src="./pic4.jpg"/>
      </transition>
      <h2 class="h2 font serif text-xl mt-12">Que sepas que siempre estaremos todos para ti, <span class="text-blue-400">te queremos Papá</span>.</h2>
      <div class="flex justify-center mt-10 text-2xl">We

<svg class="heart mr-3 ml-3" viewBox="0 0 32 29.6">
  <path d="M23.6,0c-3.4,0-6.3,2.7-7.6,5.6C14.7,2.7,11.8,0,8.4,0C3.8,0,0,3.8,0,8.4c0,9.4,9.5,11.9,16,21.2
  c6.1-9.3,16-12.1,16-21.2C32,3.8,28.2,0,23.6,0z"/>
</svg> 

You</div>
  </div>
  <div class="flex justify-self-center justify-center align-middle content-center w-full h-7 mt-24 bg-blue-400"><span class="text-gray-900">Desarrolado por <a class="text-green-700" href="htpps://twitter.com/kevincotodev=09">Kevin Coto</a></span></div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}


.profile{
  width: 200px;
  height: 200px;
}
.h2{
  width:300px
}
.image{
  width: 300px;
  height: 200px;
}
.top-appear-class{
	opacity: 0;
  
}

.top-appear-active-class{
	transition: all 1.5s;
  transform: translateY(-20px);
  opacity: 0;
}

.top-appear-to-class{
	opacity: 1;
  transform: translateY(0px)
}
.bottom-appear-class{
	opacity: 0;
  
}

.bottom-appear-active-class{
	transition: all 1s;
  transform: translateY(20px);
  opacity: 0;
}

.bottom-appear-to-class{
	opacity: 1;
  transform: translateY(0px)
}

.left-appear-class{
	opacity: 0;
  
}

.left-appear-active-class{
	transition: all 1.5s;
  transform: translateX(-50px);
  opacity: 0;
}

.left-appear-to-class{
	opacity: 1;
  transform: translateX(0px)
}
.heart {
  fill: red;
  position: relative;
  top: -40px;
  width: 50px;
  animation: pulse 1s ease infinite;
}

@keyframes pulse {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.3);
  }
  100% {
    transform: scale(1);
  }
}
</style>
