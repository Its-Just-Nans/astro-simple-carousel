# astro-simple-carousel &middot; [![npm version](https://img.shields.io/npm/v/astro-simple-carousel)](https://www.npmjs.org/package/astrosim--barchart) [![download count](https://img.shields.io/npm/dw/astro-simple-carousel)](https://www.npmjs.org/package/astro-simple-carousel)

A simple carousel in Astro

- npm: <https://www.npmjs.com/package/astro-simple-carousel>
- demo here: <https://its-just-nans.github.io/astro-simple-carousel/>

This package relies heavily on the `Astro.slots` API. To add an element to the carousel, you need to add a slot attribute to the element. The carousel will then display the elements in the order of the slot name.

## Usage

```astro
---
import Carousel from "astro-css-carousel";
import { Image } from "astro:assets";
---

<Carousel>
    <div slot="1">
        <p>put whatever you want</p>
        <img src="https://picsum.photos/200/200?random=1" alt="song" />
    </div>
    <Image height={300} width={300} src={"https://picsum.photos/200/200?random=2"} alt="Astro" slot="2" />
    <div class="styled" slot="3">
        <img src="https://picsum.photos/200/200?random=4" alt="song" />
        <p>bring your own style into the carousel element</p>
    </div>
    <Image height={300} width={300} src={"https://picsum.photos/200/200?random=3"} alt="Astro" slot="4" />
</Carousel>
```

## License

Licensed under the MIT License - [LICENSE](LICENSE)
