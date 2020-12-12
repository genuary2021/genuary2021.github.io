# Prompts

## JAN.1

```
// TRIPLE NESTED LOOP
```

---
## JAN.2

[Rule 30](https://www.wolframalpha.com/input/?i=rule+30) (elementary cellular automaton)[https://en.wikipedia.org/wiki/Elementary_cellular_automaton]

---
## JAN.3

Make something human.

---
## JAN.4

Small areas of symmetry.

---
## JAN.5

Do some code golf! How little code can you write to make something interesting? Share the sketch and its code together if you can.

---
## JAN.6

Triangle subdivision.

---
## JAN.7

Generate some rules, then follow them by hand on paper.

---
## JAN.8

Curve only.

---
## JAN.9

Interference patterns.

---
## JAN.10

```
// TREE
```

---
## JAN.11

Use something other than a computer as an autonomous process (or use a non-computer random source).

---
## JAN.12

Use an API (e.g. the weather). Here's [a huge list of free public APIs](https://github.com/public-apis/public-apis).

---
## JAN.13

Do not repeat.

---
## JAN.14

```
// SUBDIVISION
```

---
## JAN.15

Let someone else decide the general rules of your piece.

---
## JAN.16

Circles only

---
## JAN.17

Draw a line, pick a new color, move a bit.

---
## JAN.18

One process grows, another process prunes.

---
## JAN.19

Increase the randomness along the Y-axis.

---
## JAN.20

No loops.

---
## JAN.21

```
function f(x) { 
    DRAW(x); 
    f(1 * x / 4); 
    f(2 * x / 4); 
    f(3 * x / 4); 
}
```

---
## JAN.22

Draw a line. Wrong answers only.

---
## JAN.23

<b style="background-color: #264653">#264653</b>
<b style="background-color: #2a9d8f">#2a9d8f</b>
<b style="background-color: #e9c46a">#e9c46a</b>
<b style="background-color: #f4a261">#f4a261</b>
<b style="background-color: #e76f51">#e76f51</b>, no gradients. 

Optionally, you can use a black or white background.

---
## JAN.24

500 lines.

---
## JAN.25

Make a grid of all the permutations of something.

---
## JAN.26

2D Perspective.

---
## JAN.27

Gradients without lines.

---
## JAN.28

Use sound.

---
## JAN.29

Any shape, none can touch.

---
## JAN.30

Replicate a natural concept (e.g. gravity, flocking, path following).

---
## JAN.31

```
10 SEARCH FOR "ENO'S OBLIQUE STRATEGIES"
20 OBTAIN ONE
30 THAT IS YOUR PROMPT FOR TODAY
```

---

<script>
    // Uncomment the `if` line to highlight days only in january 2021
    function setHighlight () {
        const now = new Date();
        console.log(now.getFullYear(), now.getMonth());
        if (now.getFullYear() !== 2021 || now.getMonth() !== 0) return;
        const hash = "#jan" + now.getDate();
        if (!document.location.hash) document.location = hash;
        document.querySelector(hash).classList.add("today");
    }

    // Make sure we aren't trying to do this before
    // the browser has loaded the whole page
    addEventListener('load', setHighlight);
</script>
