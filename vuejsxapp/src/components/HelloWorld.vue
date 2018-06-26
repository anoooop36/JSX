
<script lang = 'tsx' >
import Vue from 'vue'
import { Component } from 'vue-property-decorator'
import TextComponent from './TextComponent.vue'
export default class HelloWorld extends Vue {
  name: 'HelloWorld'
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
  render (createElement) {
     return (
         <div>
         <button domPropsInnerHTML={this.msg} onClick={this.handleClick}></button>
         <TextComponent></TextComponent>
         </div>
     )
 }
  handleClick () {
    alert('button clicked')
  }
}
</script>

