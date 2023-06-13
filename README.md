# Shopify: Products recommendations slider section

![Preview](https://github.com/qcyGH/Shopify--Products-recommendations-slider-section/blob/main/images_for_git/preview.png "Preview")

## Description

This is product recommendation section with slider (Swiper.js). Its take products from Shopify API and then displays them in slider.

Settings:

- Label text

 Card settings

 - Show secondary image while hover.
 - Show rating in card.

 Slider settings

 - Max product range.
 - Transition animation.
 - Slider speed. (transition duration)
 - Enable slider autoplay
 - Slider autoplay delay

## How to use

1. Download project
2. Past all from `section` folder to your theme folder.
3. If you dont use Swiper in your project, you need to connect the `swiper-bundle.min.css` and `swiper-bundle.min.js` files in `layout/theme.liquid` like this:

```liquid
<head>
 ...some code

 {{ 'swiper-bundle.min.css' | asset_url | stylesheet_tag }}

 ...some code

 <script src="{{ 'swiper-bundle.min.js' | asset_url }}"></script>

 ...some code
</head>
```

4. To adapt this section to your theme, you can change the styles in file `assets/slider-horizontal.css`. You also need to select the size of the image in the `product card` (if you want to use my product card snippet), this can be done in `nippets/produt-card.liquid` in lines 5 and 7.
5. Add section to page.
6. Configure section in theme editor.
7. Enjoy (～￣▽￣)～

P.s. I used Bootstap 5 Grid, so if you using another grid system, change html in `sections/product-recommendation.liquid`.
P.P.s.\ My project include product-card snippet, so if you dont need this, you can delete this file and use your snippet instead.

## Code

### Section
![Section](https://github.com/qcyGH/Shopify--Products-recommendations-slider-section/blob/main/images_for_git/section.png "Section")

### Product card
![Product card](https://github.com/qcyGH/Shopify--Products-recommendations-slider-section/blob/main/images_for_git/card.png "Product card")

### Script

This script retrieves products from the Shopify API and then gives them to the slider. 
![Script](https://github.com/qcyGH/Shopify--Products-recommendations-slider-section/blob/main/images_for_git/script.png "Script")
