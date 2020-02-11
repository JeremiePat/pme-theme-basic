# StuffMe Theme: Basic

This is a basic theme to be used with [**StuffMe**](https://github.com/JeremiePat/stuffme)

## Install

```bash
$ npm i stuffme-theme-basic -g
```

## Usage

```bash
# Serve your slides
$ stuff serve -t stuffme-theme-basic

# Create your slide as a standalone file
$ stuff make -t stuffme-theme-basic
```

## Customize your slides

This basic theme provide many CSS classes that you can applied to your slides
or elements to customize their layout.

### Layout

> **NOTE:** _Some classes have effect only in combination with other classes.
> In such cases, the whole dependency chain is provided. For example,
> `.grid.col-1-2` means that the class `.col-1-2` has effect only if it's set
> on a slide or element with the class `.grid`_

| Class              | Slide | Element | Description |
|:-------------------|:-----:|:-------:|:------------|
| .left              | x | x | Align the whole content to the left of the slide or of the element.    |
| .center-h          | x | x | Center the whole content horizontally within the slide or the element. |
| .right             | x | x | Align the whole content to the right of the slide or of the element.   |
| .top               | x | x | Align the whole content to the top of the slide or of the element.     |
| .center-v          | x | x | Center the whole content vertically within the slide or the element.   |
| .bottom            | x | x | Align the whole content to the bottom of the slide or of the element.  |
| .grid              | x |   | Apply a 2 column layout on a slide where the title (if any) is on top, and the 2 next elements are placed side by side. |
| .grid.title-left   | x |   | Put the title on the left side of the slide (it will be rotated to appear vertical)  |
| .grid.title-right  | x |   | Put the title on the right side of the slide (it will be rotated to appear vertical) |
| .grid.title-bottom | x |   | Put the title at the bottom of the slide |
| .grid.col-1-2      | x |   | Tweak the 2 column layout to have the 2nd column twice the size of the 1st one. |
| .grid.col-2-1      | x |   | Tweak the 2 column layout to have the 1st column twice the size of the 2nd one. |
| .grid.col-1-1-1    | x |   | Apply a 3 column layout on a slide where the title (if any) is on top, and the 3 next elements are placed side by side. |
| .grid.col-1-1-2    | x |   | Tweak the 3 column layout to have the 3rd column twice the size of the other two. |
| .grid.col-1-2-1    | x |   | Tweak the 3 column layout to have the 2nd column twice the size of the other two. |
| .grid.col-2-1-1    | x |   | Tweak the 3 column layout to have the 1st column twice the size of the other two. |

### Font size

Font size modifiers, when they are applied on a slide, change the font size of
all children in a way that preserves the relative size difference between each
children. However, when applied on elements they force the size regardless of
any context.

| Class     | Slide | Element | Description |
|:----------|:-----:|:-------:|:------------|
| .font-xxl | x | x | Increase the font size to the largest size available.  |
| .font-xl  | x | x | Increase the font size to an extra large size. |
| .font-l   | x | x | Increase the font size to a larger size. |
| .font-m   | x | x | Set the font size to a medium size. This is the default font size applied to the document. |
| .font-s   | x | x | Decrease the font size to a smaller size. |
| .font-xs  | x | x | Decrease the font size to an extra small size. |
| .font-xxs | x | x | Decrease the font size to the smallest size available. |

### Special cases

| Class      | Slide | Element | Description |
|:-----------|:-----:|:-------:|:------------|
| .margin    | x | x | Add an extra bottom margin to elements. This is usually used to mimic a paragraph structure when list are tweaked with the `.no-bullet` class. |
| .no-bullet | x | x | Remove the bullets from `<ul>` and `<ol>` elements. |
| .plain     |   | x | Remove border and background from targeted `<img>` elements. |
| .stretch   |   | x | Force an element to be maximized in size while fitting within the slide. it is usually applied to image, iframe, video or code block. |
