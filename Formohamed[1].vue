<template>
        <div class="flex flex-col  py-[100px] space-y-4">
            <div class="w-full">
                <div @click="toggle($event)" class=" w-full bg-gray-200 text-gray-600 flex flex-row justify-between p-4">2017</div>
                <div class="mySlides hidden">jejbefkejbfkjefbkjebfkjebfkjebfkjebfkjbekjfbekjfbekjfbekjbfkjebfkejbfkejbfkjefbke</div>
            </div>
                        <div id="s1" >
                <div @click="toggle($event)" class="bg-gray-200 text-gray-600 flex flex-row justify-between p-4">2018</div>
                <div  class="mySlides hidden"  >jejbefkejbfkjefbkjebfkjebfkjebfkjebfkjbekjfbekjfbekjfbekjbfkjebfkejbfkejbfkjefbke</div>
            </div>
                        <div id="s1">
                <div @click="toggle($event)" class="bg-gray-200 text-gray-600 flex flex-row justify-between p-4">2019</div>
                <div class="mySlides hidden" >jejbefkejbfkjefbkjebfkjebfkjebfkjebfkjbekjfbekjfbekjfbekjbfkjebfkejbfkejbfkjefbke</div>
            </div>
                        <div id="s1">
                <div @click="toggle($event)" class="bg-gray-200 text-gray-600 flex flex-row justify-between p-4">2020</div>
                <div  class="mySlides hidden">jejbefkejbfkjefbkjebfkjebfkjebfkjebfkjbekjfbekjfbekjfbekjbfkjebfkejbfkejbfkjefbke</div>
            </div>
        </div>

</template>
<script>
export default {
    data(){
        return{

        }
    },
    methods :{
        toggle(event){
            var y = document.getElementsByClassName("mySlides");
                    var i;
  for (i = 0; i < y.length; i++) {
      if(y[i] == event.target.nextSibling){
     console.log('')
      }
      else{
         y[i].classList.replace('block','hidden') 
      }
  }
      if(event.target.nextSibling.classList.contains('hidden') ){
         event.target.nextSibling.classList.replace('hidden','block') 
      }
      else{
           event.target.nextSibling.classList.replace('block','hidden') 
      }

    

   
           
    
        }

    }
}
</script>