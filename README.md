# ghostframe css

## Lightwieght Responsive CSS boilerplate

ghostframe was developed to be used as a responsive, lightweight, low-overhead css boilerplate. 
ghostframe does not style any elements, it only contain classes used to position elements in the screen. 
A couple of alignment classes are also avaiable, but are named to not interfere with the default behaviour of any element, class or framework. 

Current unminified overhead: **2 KB**


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

**gridF** - _grid Full width_: Uses 100% width of the viewport.

**gridL** - _grid landscape_: Maximum width: 1280px.

**gridP** - _grid portrait_: Maximum width: 960px.


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
<div class="h-c">This will be horizontally center aligned</div>
<div class="h-l">This will be horizontally left aligned</div>
<div class="h-r">This will be horizzontally right aligned</div>
```

## Padding Classes:
There are padding classes avaiable to pad the content in %. 

### Padding Top
pt-05, pt-10, pt-15, pt-20
### Padding Bottom
pb-05, pb-10, pb-15, pb-20
### Padding Left
pl-05, pl-10, pl-15, pl-20
### Padding Right
pr-05, pr-10, pr-15, pr-20

Example:
```html
<div class="pt-05 pb-05">
	This contented will be padded 5% from the top (pt-05) and 5% from the bottom (pb-05)
</div>
```

## Height Classes:
There are height classes, to manually set the height of a column. 
These are named h-X, where X is the % of the viewport. It goes in increments of 10.
So, the classes are:
```css
.h-10 /* 10% of viewport height */
.h-20 /* 20% of viewport height */
.h-30 /* 30% of viewport height */
.h-40 /* 40% of viewport height */
.h-50 /* 50% of viewport height */
.h-60 /* 60% of viewport height */
.h-70 /* 70% of viewport height */
.h-80 /* 80% of viewport height */
.h-90 /* 90% of viewport height */
.h-100 /* 100% of viewport height */
```

## Other tips
You mix and match classes to better suit your layout, so don't be affraid to use them.

```html
<div class="gridP pl-05 pr-05"> <!-- Creates a grid Portrait with 5% padding on both sides -->
	<div class="r"> <!-- new row -->
		<div class="c20 h-c pt-10"> <!-- full width div with centralized text and top padding of 10% -->
			CONTENT GOES HERE
		</div>
	</div>
```

Also, feel free to mix ghostframe classes with your own custom css, that's the idea of having it be non-intrusive on other elements.
```html
<div class="gridL bg-red"> <!-- Creates a landscape grid with a custom bg-red class -->
	<div class="r"> <-- new row -->
		<div class="c5 h-r font-white font-typography"> <!-- Creates a column with custom font-white and font-typography classes -->
			CONTENT
		</div>
		<div class="c15 h-r pl-10 font-black font-anotherfont"> <!-- Another column with different styling classes -->
			MORE CONTENT
		</div>
	</div>
</div>
```

ghostframe can integrate into any custom css code, regardless of the type. 
It shouldn't be used to style objects or elements, the idea is to provide a skeleton frame for the structure of the page, only.
You can even integrate ghostframe with bootstrap, although there's little reason to do that, since it was developed exactly to be a lightweight, non-intrusive alternative to Bootstrap.

## Known Bugs 
None. 