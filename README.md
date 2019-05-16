# vue-owlcarouselbox

## Install

#### NPM 

Install the package:

```
npm i vue-owlcarouselbox
```
## Usage

```html
<div class="container-fluid max-content">
    <no-ssr>
        <Owl :options="options">
            <div class="item">
                <img src="http://fpoimg.com/600x250/For%20Place%20Only%20Image" alt="">            
            </div>
            <div class="item">
                <img src="http://fpoimg.com/600x250/For%20Place%20Only%20Image" alt="">            
            </div>
        </Owl>
    </no-ssr>
</div>
```

```javascript

    import Owl from 'vue-owlcarouselbox';

    export default {
        components: {
            Owl: Owl
        },
        data() {
            return {
                options: { //https://owlcarousel2.github.io/OwlCarousel2/demos/basic.html
                    items: 1,
                    autoplay: false,
                    loop: true,
                    items: 1,
                    margin: 0,
                    nav:true,
                    dots:false
                }
            }
        },
    }


```
