<template>
 <div class="wrapper">
		<div class="control">
		  <ul>
		  <li v-for="(message, index) in messagesBank">
		  <input class="input" type="text" placeholder="Text input" :value=message.text :name="'message'+index.toString()"  v-model="message.text">
		  </li>
		</div>
		<button @click="show">Click</button>

 </div>
 	

</template>

<script>
export default {
  name: 'messages',
  components: {
   
  },
  data () {
    return {
    	messagesBank: [
    	{text:'message1'},
    	{text:'message2'},
    	{text:'message3'},
    	{text:'message4'}

		]
    }
  },
  methods : {
  	show: function() {
  		console.log(this.messagesBank);
  	}
  }
  

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
