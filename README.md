# pull-delete
This is a sliding delete small plug-in for mobile terminal development, depending on jQuery!


## Usage:
### Import JS and CSS files
The files you need are in the res directory. When you use them, you can import `pulldelete.js` and `pulldelete.css`
Check out `index.html` as a working prototype

### Init library in your code
#### Default delete button
```
$('.pull_delete').pulldelete(function($dom){
    // something you want here
    console.log('click delete');
    $dom.remove();
});
```

#### Custom buttons
```
const target_element = 'pull_pin';  // implementing pins instead of delete
$('.' + target_element).pulldelete(function($dom){
    // something you want here
    console.log('click pin');
    $dom.remove();
}, target_element);
```
But with a custom `pull_pin` class to inherit styling from `pull_delete` use `pull_delete_css` class:
```
<div class="pull_pin pull_delete_css">...</div>
```
