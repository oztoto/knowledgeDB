```scss
@function getvw($size, $viewport: 320) {
  $rate: 100 / $viewport;
  @return $rate * $size * 1vw;
}

@use "foundation/mixin" as mi;
height: mi.getvw(10);
```