# Jquery Cuteness Adder

jQuery plugin that adds a sprite that follows the cursor

## Demo
<https://FiDyA-dev.github.io/jquery_cuteness_adder/example>

## Usage
Include jQuery and the plugin.
```html
<script src="js/jquery.js"></script>
<script src="js/jquery_cuteness_adder.min.js"></script>
```
Initialize the plugin.
```js
$('document').ready(function() {
  $('.some-block').addCuteness();
});
```

## Settings

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Type&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Default&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
| ---- | ---- | ---- | ---- |
| speed | int | 3 | Sprite move speed |
| color | string | '' | Sprite color in HEX format: `'#000000'`, `'#2780E3'`. If the given value is not a color, then the color will be generated randomly |
| sprite | string | '' | Sprite selection. This setting can take one of the following values: `'cat'`, `'dog'`, `'dino'`. If another value is set, then a random sprite will be selected |

## Example with Options
This example will create a green cat on a block with class `some-block` 
```js
$('document').ready(function() {
  $('.some-block').addCuteness({
    speed: 4,
    color: '#00ff00',
    sprite: 'cat'
  });
});
```
