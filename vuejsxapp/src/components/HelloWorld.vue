
<script>
import TextComponent from './TextComponent.vue'
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  render (createElement) {
     return (
         <div>
         <button domPropsInnerHTML={this.msg} onClick={this.handleClick}></button>
         <TextComponent></TextComponent>
         </div>
     )
 },
 methods: {
   handleClick () {
     alert('button clicked')
   }
 }
}
</script>

