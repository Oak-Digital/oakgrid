
# OAKGrid
Simple Lightweight CSS Grid Template

## DEMO
[https://codepen.io/plenge/pen/zYvExRY](https://codepen.io/plenge/pen/zYvExRY)

## Table of contents
- [Naming Convention](#Naming-conventions-based-on-Bootstrap)
- [Example of grid markup](#Example-of-grid-markup)
- [How to use rows](#The-use-of-`.row`)
- [How to offset columns](#Offset)
- [Making it responsive](#Making-it-responsive)

___

## Naming conventions based on Bootstrap

For the sake of easy transition for anyone already familiar with Bootstrap, the class naming convention is almost identical to Bootstrap 4.

## Example of grid markup

To create a grid, you only need to create a `.grid` wrapper, with `col-*` childrens. 

The number following `.col-` represents the amount of columns the given element should span.

**Minimum Markup Example:**
```
<div class="grid">
    <div class="col-4">
        Content goes here
    </div>        
    <div class="col-4">
        Content goes here
    </div>        
    <div class="col-4">
        Content goes here
    </div>        
</div>
```

## The use of `.row`

Rows can be added to the grid to ensure that content is vertically seperated.

*Rows are completely optional in the markup*

**Example of markup WITHOUT a `.row` element**

```
<div class="grid">
    <div class="col-6">
        This is 6 columns
    </div>        
    <div class="col-6">
        Content goes here
    </div>        
</div>
```

// TODO: IMAGEHERE
As you can see in the above example, the grid behaves as expected. But what if we don't want the 2 columns in the same row, but still want to contain the 6 column width.

That is where `.row` comes into play

**Example of markup WITH a `.row` element**
```
<div class="grid">
    <div class="row">
        <div class="col-6">
            This is 6 columns
        </div>        
        <div class="col-6">
            Content goes here
        </div>        
    </div>
</div>
```

// TODO: IMAGEHERE

By adding row elements, we ensure that the elements are seperated vertically.

## Offset
It it possible to offset columns, in case you need something aligned differently.

**Example of offset**
```
<div class="grid">
    <div class="row">
        <div class="col-6">
            This is 6 columns
        </div>        
        <div class="col-6">
            Content goes here
        </div>        
    </div>
</div>
```


## Making it responsive

The basic `.col-*` class, will always stay on the same amount of columns, no matter the viewport size.

To change the grid layout for different devices you can use responsive selectors instead.

Responsive naming:

 -| Default | Small (>576) | Medium (>576) | Large (>576) | Extra large (>576)
 ------ | ------ | -------- | -------- | -------- | --------
**Col prefix** | `col-` | `col-sm-` | `col-md-` | `col-lg-` | `col-xl-`
**Offset prefix** | `offset-` | `offset-sm-` | `offset-md-` | `offset-lg-` | `offset-xl-`


___ 
## Have you used OAKGrid for a project?
-- Tell us, and we will gladly highlight your project here.