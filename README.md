
# @jupa-dev/vue-slider
SLIDER VUE / NUXT

## Installation



```bash
  npm i @jupa-dev/vue-slider
```
    
## Usage/Examples

```javascript
// nuxt.config.js
plugins: [
    { src: '~/plugins/vue-slider', mode: 'client' },
  ],

// vue-slider.js
import Vue from 'vue'
import { Swiper, Slide } from "@jupa-dev/vue-slider/src/components";

Vue.component('Swiper', Swiper)
Vue.component('Slide', Slide)


// Component
<Swiper v-if="list.length > 0">
  <Slide v-for="(item,index) in list" :key="index">
  </Slide>
</Swiper>

```

## API

| Prop          | Funcionalidad                    | Default value |
| ------------- | ------------------------ | ---- |
| autoPlay      | rotar automáticamente             | true |
| showIndicator | mostrar el punto del carrusel     | true |
| interval      | frecuencia desplazamiento     | 2500 |
| duration      | duración | 500  |

```javascript
✅  Funcionalidades Swiper : <Swiper ref="swiper"></Swiper>

    ✅  this.$refs.swiper.prevSlide();  anterior
    ✅  this.$refs.swiper.nextSlide();  siguiente
    ✅  this.$refs.swiper.slideTo(2);  ir
```
