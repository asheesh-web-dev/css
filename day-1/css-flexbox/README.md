# css flex-box

components of **flex-box** layout

1. **flex-container**
2. **flex-item**

## flex-container

define `flex-container` with `display:flex` property.

### `flex-container` properties

1. **`flex-direction`:** row(default), column, row-reverse, column-reverse
2. **`flex-wrap`:** wrap, no-wrap(default)
3. **`flex-flow`** shorthand for `flex-direction` and `flex-wrap`
4. **`justify-content`**
   1. align items along main axis
   2. center, flex-start(default), flex-end, space-arround, space-between, space-evenly
5. **`align-items`**
   1. align items along cross axis
   2. normal(default), stretch, centre, flex-start, flex-end, baseline
6. **`align-content`**
   1. align flex-lines. works only on flex-items wrap onto multiple lines
   2. strech(default), center, flex-start, flex-end, space-between, space-around, space-evenly

## flex-items

The direct children of flex-container

### `flex-item` properties

1. **`flex-grow`:**
   1. how much flex items will grow relative to rest of flex-items. defualt value is `0`.
   2. the ramaining sapce is proportionally distributed for items.
      1. `flex-grow:1` for an item while all other items have `flex-grow:0` will make the item to take all the space.
2. **`flex-shrink`:**
   1. how much an item will shrink
   2. default value is `1` ie **shrink all items equally**
3. **`flex-basis`:**
   1. length of flex-item
   2. > > don't use `width` to set length of flex-items use `flex-basis`
4. **`flex`**: short hand for `flex-grow` , `flex-shrink` & `flex-basis`
