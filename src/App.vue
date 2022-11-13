<template>
    <div id="app">
    	  <a class="button" href="#" data-title="Free download">
            <span>
              <span>Free download</span>
            </span>
          </a>
    </div>
</template>

<script>

export default {
  name: 'App',
  components: {
   
  },
  
</script>

<style lang="scss">


.button{
    display: block;
    position: relative;
    height: 3.4em;
    width: 10em;
    margin: .7em auto;
    overflow: hidden;
    text-decoration: none;
  }
  
  .button > span{
    display: block;
    position: absolute;
    overflow: hidden;
      left: 0;
      top: 0;
      width: 0%;
      height: 100%;
      transition: 1s ease-in-out; 
  }
  
  .button:after, .button > span > span {
    display: block;
    text-align: center;
    border-radius: 0.625em;
    padding: 1em 0; }
  .button:after {
    content: attr(data-title);
    width: 100%;
    background: #4186b2;
    color: #e26961; } 
  .button > span > span {
    width: 10em;
    background: #e26961;
    color: #4186b2; }
  
  /* what happens on hover */ 
  .button:hover > span {
    width: 100%; }
  
</style>
