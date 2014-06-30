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