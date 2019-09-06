# Pure CSS Material Design Buttons ![alt text](https://img.shields.io/badge/CSS--blue "CSS") ![alt text](https://img.shields.io/badge/HTML5--blue "CSS")
 See it in action https://mbotha.github.io/css-md-buttons



 
 #### Very minimal CSS only Material design buttons
## HTML to display the button

```html
<button type="button" class="bg-blue waves">button</button>
```
## CSS to generate the waves effect

```css
        .waves {
            position: relative;
            overflow: hidden;
            transform: translate3d(0, 0, 0);
        }
        .waves:after {
            content: "";
            display: block;
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
            background-image: radial-gradient(circle, #fff 10%, transparent 10.01%);
            background-repeat: no-repeat;
            background-position: 50%;
            transform: scale(10, 10);
            opacity: 0;
            transition: transform .5s, opacity 1s;
        }
        .waves:active:after {
            transform: scale(0, 0);
            opacity: .3;
            transition: 0s;
        }
 ```
        

