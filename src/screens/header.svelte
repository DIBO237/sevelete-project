<script>
  let anu = 0
  let start = false
  let timers = 0

const anuCount = ( )=>{

   if(start){
   
    anu++

   }  
  
    
}

const time = ()=>{
          timers++
          //console.log(timers)
      }

const startShow = ()=>{
     anu = 0
      start = true
      console.log(start)
      
     

     let cleartime= setInterval(time,1000)

      setTimeout(()=>{
        start = false
         timers = 0
         
         clearInterval(cleartime)
         
         
    }, 6000)
     

      
       
}


const anuNeg = ( )=>{
   if(anu !=0){
    anu--
   }
    
}





</script>

<div>
    <h2>TIMER {timers}</h2>
</div>


<div>
    <h2>TOTAL: {anu}</h2> 
 </div>
 



<button on:click={anuCount}>

    <h1>
      Click
    </h1>
</button>


<!-- <div>
   <h2>{anu}</h2> 
</div> -->


<!-- <div on:click={star}>

    <h1>
      MINUS -
    </h1>
</div> -->

<button on:click={startShow}>
  <h5>Start</h5>
</button>