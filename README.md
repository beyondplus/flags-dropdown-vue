# flag-dropdown-vue
Flag Dropdown Component for Vue2

# Html
`<flags-dropdown  v-on:change="optionSelected" :selected="selectedValue"></flags-dropdown>`

# Script
`
import { FlagsDropdown } from 'flags-dropdown-vue'
var app = new Vue({
    el: '#app',
    data: {
      selectedValue : "mm"
    },
    components: {
      FlagsDropdown
    },
    methods: {
    	optionSelected: function (data) {
            this.selectedValue = data
      }
    }
});
`

