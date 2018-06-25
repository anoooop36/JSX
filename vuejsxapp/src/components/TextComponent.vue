
<script>
export default {
  name: 'TextComponent',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
 render (createElement) {
     const inputAttributes = {
         class: 'input-field has-outline', // class definition
         onClick: this.handleClick, // event handler
         backdrop: false // custom prop
     }
     const inputMarkup = this.multiline
         ? <textarea {...inputAttributes}></textarea>
         : <input {...inputAttributes}/>

    return inputMarkup
 },
 methods: {
   handleClick () {
     alert('button clicked')
   }
 }
}
</script>

