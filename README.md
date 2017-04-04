# flag-dropdown-vue
Flag Dropdown Component for Vue2

# Installation
npm install flags-dropdown-vue --save


## Usage
```javascript
import FlagsDropdown from 'flags-dropdown-vue'
Vue.component('flags-dropdown', FlagsDropdown);

var app = new Vue({
    el: '#app',
    data: {
      country_iso : "mm"
    },
    methods: {
    	optionSelected: function (data) {
            //console.log(data.id)
            //console.log(data.phonecode)
            this.country_iso = data.iso
      }
    }
});
```

# Html
```html
<link rel="stylesheet" type="text/css" href="css/flags.min.css">
<link rel="stylesheet" type="text/css" href="css/custom.css">
<script  src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.2.6/vue.min.js"></script>
<flags-dropdown  v-on:change="optionSelected" :selected="country_iso"></flags-dropdown>
```
