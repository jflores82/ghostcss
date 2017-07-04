# ghostframe css

## Lightwieght Responsive CSS boilerplate

ghostframe was developed to be used as a responsive, lightweight, low-overhead css boilerplate. 
ghostframe does not style any elements, it only contain classes used to position elements in the screen. 
A couple of alignment classes are also avaiable, but are named to not interfere with the default behaviour of any element, class or framework. 


## Usage 
Load the stylesheet into your HTML file
```html
<link rel="stylesheet" href="css/ghostframe.css">
```


Create a grid, some rows and columns
```html
<div class="gridL"> <!-- Create the Grid -->
	<div class="r"> <!-- Create a row -->
		<div class="c10"> <!-- This column takes half of the grid -->
			Your Content
		</div>
	</div>
</div>
```

You can organize your content through the grid as necessary.


## Responsiveness:
You can use 3 different grid sizes, to better fit your content.

gridF - Uses 100% width of the viewport.
gridL - Maximum width: 1280px
gridP - Maximum width: 960px

Columns will stay side by side when the resolution's width are greater than 960px.
When it dips below 960px it will stack columns 2 by 2, independent of the original column size.
If the width drops below 550px columns will be stacked 1 by 1.

There are 20 columns avaiable, you can have a mix and match of columns, up to a max of 20:
```html
<div class="c1">Something</div> 
<div class="c19">Something Else</div>
```

```html
<div class="c15">Something</div>
<div class="c4">Something Else</div>
<div class="c1">Other content</div>
```

You don't need to use all 20 columns:
```html
<div class="c12">Something</div>
<div class="c1">Something Else</div>
```

## Aligment Classes:
You can use the following classes to align content:
```html
<div class="t-c">This will be center aligned</div>
<div class="t-l">This will be left aligned</div>
<div class="t-r">This will be right aligned</div>
```

## Padding Classes:
There are padding classes avaiable to pad the content in %. 

### Padding Top: pt-05, pt-10, pt-15, pt-20
### Padding Bottom: pb-05, pb-10, pb-15, pb-20
### Padding Left: pl-05, pl-10, pl-15, pl-20
### Padding Right: pr-05, pr-10, pr-15, pr-20

```html
<div class="pt-05 pb-05">This contented will be padded 5% from the top (pt-05) and 5% from the bottom (pb-05)</div>
```


## Known Bugs 
None. 