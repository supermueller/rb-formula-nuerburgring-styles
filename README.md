Flipping Cards Panel
====================

## Vorraussetzungen

- Das Panel (*Rail of Feed Cards*) muss die ID `flippingCards` (*HTML id*) und die Klasse `flippingCards` (*Additional CSS Classes for Theming*) haben.
- Vor dem Flipping-Cards-Panel sind die CSS-Importing-Panels "Flipping Cards Settings" und "Flipping Cards Styles" eingebunden (Quellcode siehe unten).
- Nach dem Flipping-Cards-Panel ist das Custom-Scripts-Panel "Flipping Card Script" eingebunden (Quellcode siehe unten).
- Es können auch mehrere Panels in einer Even-Page benutzt werden, allerdings müssen sich die ID (z.B. `driverPanel` und `carPanel`) dann unterscheiden. **Achtung:** Die Klasse bleibt aber bei allen Panels gleich (`flippingCards`).

## Scripts und Styles

### Flipping Card Settings

⚠️ Zum Anpassen der Karten muss nur dieser Code geändert werden.

```css
#flippingCards {
    --slide-1: url("https://img.redbull.com/image/upload/redbullcom/2023/6/16/wsxraimwlymcqno8hgpo");
    --slide-2: url("https://img.redbull.com/image/upload/redbullcom/2023/6/16/csbympagoucsbxcrxcse");
}
```

#### Bilder hinzufügen

Zum Hinzufügen von Bildern einfach innerhalb der geschweiften Klammern eine Zeile hinzufügen, wobei beim Namen vor dem Doppelpunkt, der Zähler hochgezählt wird:

```css
#flippingCards {
    --slide-1: url("https://img.redbull.com/image/upload/redbullcom/2023/6/16/wsxraimwlymcqno8hgpo");
    --slide-2: url("https://img.redbull.com/image/upload/redbullcom/2023/6/16/csbympagoucsbxcrxcse");
    --slide-3: url("https://img.redbull.com/image/upload/redbullcom/2023/6/16/wsxraimwlymcqno8hgpo");
}
```

### Flipping Card Script

- URL of the script to execute: `https://rb-red-bullnurburgring-vp-prod.onrender.com/bundle.js`

### Flipping Cards Styles

```css
.flippingCards{background:linear-gradient(180deg, rgba(0, 15, 30, 0) 0%, rgba(0, 15, 30, 0.05) 50.81%, rgba(0, 15, 30, 0.05) 90.43%, rgba(0, 15, 30, 0) 100%);-webkit-user-select:none;-moz-user-select:none;user-select:none}.flippingCards .external-feed-card{border-radius:0;box-shadow:none;overflow:visible}.flippingCards .external-feed-card__wrapper{contain:inherit;content-visibility:visible}.flippingCards .external-feed-card__preview{border-radius:none;overflow:visible}.flippingCards .external-feed-card__info{display:none}.flippingCards .external-feed-card:hover .image-view{-webkit-transform:none;transform:none;transition:none}.flippingCards .interactive-preview-media{overflow:visible}.flippingCards .image-view{overflow:visible}.flippingCards .image-view__container{-webkit-filter:none;filter:none}.flippingCards .rail__item{aspect-ratio:.641025641}.flippingCards .external-feed-card__wrapper{aspect-ratio:.641025641;padding-bottom:0 !important}.flippingCards .external-feed-card .image-view{-webkit-perspective:1000px;perspective:1000px}.flippingCards .external-feed-card .image-view__container{position:absolute;height:100% !important;width:100% !important;left:0 !important;top:0 !important;-webkit-transform:rotateY(0deg);transform:rotateY(0deg);-webkit-transform-style:preserve-3d;transform-style:preserve-3d;transition:background-position 0s 200ms,-webkit-transform 400ms;transition:transform 400ms,background-position 0s 200ms;transition:transform 400ms,background-position 0s 200ms,-webkit-transform 400ms;transition-timing-function:cubic-bezier(0.65, 0.05, 0.36, 1);background-position:0% 50%;background-size:auto 100%;-webkit-filter:drop-shadow(0 4px 8px rgba(0, 0, 0, 0.02)) drop-shadow(0 15px 24px rgba(0, 0, 0, 0.06));filter:drop-shadow(0 4px 8px rgba(0, 0, 0, 0.02)) drop-shadow(0 15px 24px rgba(0, 0, 0, 0.06))}.flippingCards .external-feed-card .image-view__content{display:none}.flippingCards .rail__item .image-view{-webkit-transform:scale(1);transform:scale(1);transition:-webkit-transform 100ms !important;transition:transform 100ms !important;transition:transform 100ms, -webkit-transform 100ms !important;transition-timing-function:cubic-bezier(0.45, 0.05, 0.55, 0.95) !important}.flippingCards .rail__item a:active .image-view{-webkit-transform:scale(0.975);transform:scale(0.975)}.flippingCards .rail__item a[data-revealed=true] .image-view__container,.flippingCards .rail__item a:not([data-revealed=true]):focus .image-view__container{-webkit-transform:rotateY(180deg);transform:rotateY(180deg);background-position:100% 50%}@media(hover: hover){.flippingCards .rail__item a:hover .image-view__container{-webkit-transform:rotateY(180deg);transform:rotateY(180deg);background-position:100% 50%}}.flippingCards .rail__item:nth-child(1) .image-view__container{background-image:var(--slide-1, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(2) .image-view__container{background-image:var(--slide-2, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(3) .image-view__container{background-image:var(--slide-3, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(4) .image-view__container{background-image:var(--slide-4, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(5) .image-view__container{background-image:var(--slide-5, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(6) .image-view__container{background-image:var(--slide-6, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(7) .image-view__container{background-image:var(--slide-7, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(8) .image-view__container{background-image:var(--slide-8, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(9) .image-view__container{background-image:var(--slide-9, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(10) .image-view__container{background-image:var(--slide-10, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(11) .image-view__container{background-image:var(--slide-11, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(12) .image-view__container{background-image:var(--slide-12, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(13) .image-view__container{background-image:var(--slide-13, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(14) .image-view__container{background-image:var(--slide-14, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(15) .image-view__container{background-image:var(--slide-15, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(16) .image-view__container{background-image:var(--slide-16, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(17) .image-view__container{background-image:var(--slide-17, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(18) .image-view__container{background-image:var(--slide-18, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(19) .image-view__container{background-image:var(--slide-19, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}.flippingCards .rail__item:nth-child(20) .image-view__container{background-image:var(--slide-20, url("https://img.redbull.com/image/upload/redbullcom/2023/7/18/rlpjvt8mgjggf5e8zrnt"))}

```
