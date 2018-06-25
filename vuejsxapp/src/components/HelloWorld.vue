
<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  render (createElement) {
     return (
         <button domPropsInnerHTML={this.msg} onClick={this.handleClick}></button>
     )
 },
 methods: {
   handleClick () {
     alert('button clicked')
   }
 }
}
</script>

