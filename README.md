ResponseGrid
============

Simple to use flexbox grid

Usage
--------------------------------------
ResponseGrid is based on 12 columns. Inside a container with the class flex-container, there are these, labeled with the class `col-`, what size and how many columns it should take (example: `col-xs-6`).

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

There are four breakpoints: xs, sm, md, lg. It uses the mobile-first principle (you can change that in the styles.less file, just reverse the order of @sizes), so if there isn't set a class for the bigger sizes, the styles of the smaller are applied. 

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