ResponseGrid
============

For a long time, I always made for every project a responsive grid. And it was (almost) always based on the 960 grid system. Instead of using an overweight css framework for that (like bootstrap as example), I decided to build a lightweight and responsive grid based on the 960gs. 

Usage
--------------------------------------
This grid is based on 12 columns. Inside a div with the class row, there are these, labeled with .col- and the number.

```bash
<div class="row">
    <div class="col-6"></div>
    <div class="col-6"></div>
</div>
```

to produce more space between the columns, or to change the visible position there are push and pulls.

```bash
<div class="row">
    <div class="col-4"></div>
    <div class="col-7 push-1"></div>
</div>
```

For the tablet, there are 3 options. 

- Without changes, the cols just shrink. 
- With the class .reorder on the row div, the cols 1/3 become 1/2, the 1/4 also 1/2, the 1/6 to 1/3 and the 1/12 to 1/6.
- With the class .block, all cols become 100%.

```bash
<div class="row reorder">
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