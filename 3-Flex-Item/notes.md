## Flex Item

### Flex item properties

- order
- flex-grow
- flex-shirnk
- flex-basis
- flex
- align-self

---

### Order

- Control the order of items in the flex container.
- Integer value

---

### Flex grow

- Dictates what amount of the available space inside the flex container the item should take up.
- Relative to the other items in the container.
- Default value is 0 - items do not grow.
- `flex-grow` value of 1 -flex items grow evently.

---

### Flex shrink

- Dectates the shrink factor of the flex items when the default size of flex items is larger than the flex container.
- Relative to teh other items in the conatiner.
- Default value is 1.
- value: `0` => `No shirnk`

---

### Flex basis

- Set the initail size of a flex item.
- Pixels, percentages or relative units.
- Default value is `auto`.

---

### Flex

- Short hand for `flex-grow`, `flex-shrink` and `flex-basis`.

```css
.item {
  flex-grow: 2;
  flex-shrink: 5;
  flex-basis: 200px;
}
```

```css
.item {
  flex: 2 5 200px;
}
```

- flex: `flex-grow` `<flex-shrink>` `<flex-basis>`


- defalut

```css
.item {
  flex: 0 1 auto;
}
```

- flex values

```css
/* One value, unitless number: flex-grow */
flex: 2;

/* One value, width/height: flex-basis */
flex: 10em;
flex: 30px;

/* flex: none | initial | auto */
/* Two values: flex-grow | flex-basis */
flex: 1 30px;

/* Two values: flex-grow | flex-shrink | flex-basis */
flex: 2 2 10%;
```

---


### Align self

- Align the items individually.
- Values like auto, flex-start, flex-end, center and stretch.
- Overrides the align-items value of the flex container.
- default container: `stretch`
- defalut item: `auto`