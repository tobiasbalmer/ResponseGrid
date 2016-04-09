ResponseGrid
============

Simple to use grid, based on the flexible box layout module. You may wonder if it's already usable for all browsers. Well, make up your own opinion: http://caniuse.com/#search=flexbox

Usage
--------------------------------------
ResponseGrid is based on 12 columns. Inside a container with the class flex-container, there are divs, labeled with the class `col-`, what size and how many columns it should take (example: `col-xs-6`).

```bash
<div class="flex-container">
    <div class="col-xs-6">
        <div class="box">
            Content
        </div>
    </div>
    <div class="col-xs-6">
        <div class="box">
            Content
        </div>
    </div>
</div>
```

There are four breakpoints: `xs`, `sm`, `md`, `lg`. It uses the mobile-first principle, so if there isn't set a class for the bigger sizes, the styles of the smaller are applied. 

```bash
<div class="flex-container">
    <div class="col-xs-4">
        <div class="box">
            Content
        </div>
    </div>
    <div class="col-xs-4 col-sm-5">
        <div class="box">
            Content
        </div>
    </div>
    <div class="col-xs-4 col-sm-3">
        <div class="box">
            Content
        </div>
    </div>    
</div>
```

Horizontal alignment of all the children. The options are `left`, `center` and `right` (default is left). 
```bash
<div class="flex-container xs-align-center">
    <div class="col-xs-4">
        <div class="box">
            Content
        </div>
    </div>   
</div>
```

Vertical alignment of all the children. The options are `top`, `middle` and `bottom` (default is stretch). 
```bash
<div class="flex-container xs-valign-middle">
    <div class="col-xs-4">
        <div class="box">
            Content
        </div>
    </div>   
</div>
```

Vertical alignment of one single child with the options `top`, `middle` and `bottom` (default is stretch).
```bash
<div class="flex-container">
    <div class="col-xs-4">
        <div class="box xs-valign-middle">
            Content
        </div>
    </div>   
</div>
```

You don't know how many columns you need? No problem, there's a class for that. Use `col-auto` and it just align all of them in a row.
```bash
<div class="flex-container">
    <div class="col-auto">
        <div class="box">
            Content
        </div>
    </div>   
</div>
```