ResponseGrid
============

For a long time, I always made for every project a responsive grid. And it was (almost) always based on the 960 grid system. Instead of using an overweight css framework for that (like bootstrap as example), I decided to build a lightweight and responsive grid based on the 960gs. 

Usage
--------------------------------------
This grid is based on 12 columns. Inside a div with the class row, there are these, labeled with the class `col-` and the number how wide it should be.

```bash
<div class="row">
    <div class="col-6"></div>
    <div class="col-6"></div>
</div>
```

to produce more space between the columns, or to change the visible position there are `push` and `pull`.

```bash
<div class="row">
    <div class="col-4"></div>
    <div class="col-7 push-1"></div>
</div>
```

For the tablet, there are 3 options. 

- Without changes, the cols just shrink. 
- With the class `middle-reorder` on the row div, the cols 1/3 become 1/2, the 1/4 also 1/2, the 1/6 to 1/3 and the 1/12 to 1/6.
- With the class `block`, all cols become 100%.

```bash
<div class="row middle-reorder">
    <div class="col-3"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
</div>
```

```bash
<div class="row block">
    <div class="col-4"></div>
    <div class="col-8"></div>
</div>
```

On the smartphone, all the cols become 100%. But it's also possible to make the cols reorder, or even stay at the original width, with `small-reorder` and `small-stay`.

```bash
<div class="row small-reorder">
    <div class="col-3"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
</div>
```

```bash
<div class="row small-stay">
    <div class="col-3"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
</div>
```

It is also possible to hide columns or a full row (It is to remark that hiding elements on smaller viewports is a bad habbit). Just add the classes `middle-hidden` or `small-hidden` to the row or to the cols.

```bash
<div class="row small-hidden">
    <div class="col-3 middle-hidden"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
    <div class="col-3"></div>
</div>
```
