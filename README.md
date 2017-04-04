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
<link rel="stylesheet" type="text/css" href="https://rawgit.com/beyondplus/flags-dropdown-vue/master/css/flags.min.css">
<link rel="stylesheet" type="text/css" href="https://rawgit.com/beyondplus/flags-dropdown-vue/master/css/custom.css">
<flags-dropdown  v-on:change="optionSelected" :selected="country_iso"></flags-dropdown>
```

![alt text](https://github.com/beyondplus/flags-dropdown-vue/raw/master/raw/world-flags.png "World Flags Dropdown")


## Our Website

[www.beyondplus.biz](http://www.beyondplus.biz)
