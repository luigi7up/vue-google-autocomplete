This is my fork of https://github.com/olefirenko/vue-google-autocomplete

# WHY
- The original VueAutoComplete doesn't allow changing the input type. I'll change the `<input type="text">` to `<input :type="type">`
- I want the input to be limited only to numbers when focused on a mobile phone (since in Spain all post codes are numeric) 
- I need the scrollTo the top of the input when it's focused. For this to work I'll change the `this.$emit('focus');`to `this.$emit('focus', $event);`
