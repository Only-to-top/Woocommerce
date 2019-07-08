# Woocommerce

<h2>Удаление отзывов (возможности комментирования товара)</h2>

```php
// remove reviews
add_filter( 'woocommerce_product_tabs', 'sb_woo_remove_reviews_tab', 98);
function sb_woo_remove_reviews_tab($tabs) {
  unset($tabs['reviews']);
  return $tabs;
}
```
