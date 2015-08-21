alignment-vis
=============

`alignment-vis` is a web component for visualizing sequence alignment data.

To visualize the data, you must pass in the data using the `alignment` attribute. 

For example, given the sequence data: 

- accessionA PKS--KTVKST-V
- accessionB PKV-VKTVKST-V
- accessionC PK---KTVK-T-V
- accessionD PKV-VKTVK-T-V

A visualization would be created by passing in the data to the component's `alignment` property, delimited by newline characters like this: 

```html
<alignment-vis alignment="accessionA PKS--KTVKST-V\naccessionB PKV-VKTVKST-V\naccessionC PK---KTVK-T-V"></alignment-vis>
```

#Styling

There are many customizable options for styling the visualization. Highlighting is determined by whether or not a column is aligned, unaligned, and whether or not unaligned columns contain a mismatch. 

```css
.align {
  /* Your CSS here */
}

.unalign {
  /* Your CSS here */
}

.mismatch {
  /* Your CSS here */
}
```
