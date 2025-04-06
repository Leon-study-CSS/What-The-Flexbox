synced on Laptop

# What The Flexbox?!

![](https://flexbox.io/images/WTF/share.png)

Exercises for the "What The Flexbox?!" video course. Videos available at <http://flexbox.io>

## Community What The Flexbox Content

Feel free to submit a PR adding a link to your own recaps, guides or reviews!

My [gh-page](https://herminiotorres.github.io/whattheflexbox) by [@herminiotorres](https://twitter.com/herminiotorres)

## My notes

Once you define a container as flex, all it's elements become flex items

### flex-direction
- sets the main axis
- row - the main axis is from left to right (default)
- column - the main axis is from top to bottom

the other axis is the cross axis

### flex-wrap 
the flex system tries to make the elements fit on the main axis, but it also stretches out in the container

### ordering
- the default of the orders is 0. with other numbers you can group them
- good for responsive designs
- selection of items (ex when you want to copy text) still follows the order in the html

### justify-content
- how you align the items on the main axis
- basically, what to do with the space left after the one occupied by the items

### align-items
how you align the items on the cross axis
- default is strech. take into account the size of the container

### align-content
- same params as justify-content
- what is does with the extra space on the cross axis

### align-self
 - you override the global alignment on an individual case

### flex-basis
- this is the base from where growth and shrinkage starts
- if there is space left, it is distributed between the items according to flex-grow; if you shrink the container until there is no more extra space, the elements shrink according to their flex-shrink setting

### flex-grow
- when you have extra space, how much from that extra space should it take? if multiple siblings have different values the values becomes a ratio of how much each one takes up
- flex-grow of 2 takes up twice as much space as a flex-grow of 1
- `flex-grow: 0;` means: when there is extra room, don't do anything

### flex-shrink
- how the elements slim down when there is not enough space for them
- how much of itself it should give up in proportion to the other item

### flex
- shorthand for `<flex-grow flex-shrink flex-basis>`
- `flex: 1` is shorthand for `flex-grow: 1` and `flex-shrink: 1`
- sets the ratio at which the elements grow on the axis
- a `flex: 2` on an item while the others have `flex: 1` will make that item take up double the size 

