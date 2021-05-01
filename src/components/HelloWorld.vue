<template>
<div>

 <h1>{{ msg }}</h1>
<div class="intro">
<span class="icon"></span>
  <p>
    <a href="https://debanjantewary.github.io/fetchapi" target="_blank">
   Github Api fetch (react)
    </a>
    
  </p>
</div>
<div class="maincontent">

<div class="buttons">

  <button class="dbtn" @click="state.count--">Decrease</button>
  <button class="countbtn"> {{ state.count }}</button>

  <button class="dbtn" @click="state.count++">increase</button>

</div>

  <div class="counting">

  <span v-if="state.count===0">nutral</span>
  <span v-else>
    
    <span>
<span v-if="state.count>=10">
+ 10 reached
  </span>
      <span v-if="state.count>0 & state.count<10">
            Positive (under 10)
  </span>
  <span v-else-if="state.count<=-10">
  -10 reached  
  </span>
    <span v-else-if="state.count<0 & state.count>-10"> NEGETIVE
  </span>

    </span>
    
    </span>
  </div>
</div>

</div>
</template>
<script setup>
  import { defineProps , reactive} from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })


</script>

<style scoped>
a {
  color: #42b983;
  text-decoration: none;
}

.dbtn{
border: none;
background-color: green;
color: whitesmoke;
border-radius: 5px;
padding: 10px 10px;
font-size: 20px;
margin: 5px 5px;
cursor: pointer;
  }
  .counting{

    margin: 10px;
  }

  .countbtn{

 border: none;
background-color: rgb(5, 4, 14);
color: whitesmoke;
border-radius: 5px;
padding: 10px 10px;  
font-size: 30px; 
  }

  span {
font-size: 30px;
    }

.intro{

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
    .icon{

        background: url("https://oflisback.github.io/react-favicon/img/github.ico");
        height: 30px;
        width: 32px;
       
        display: inline;

        
    }
</style>


