## 1. (9♥)

Increase the randomness along the Y-axis

---
## 2. (9♥)

No loops

---
## 3. (8♥)

<b style="background-color: #264653">#264653</b>
<b style="background-color: #2a9d8f">#2a9d8f</b>
<b style="background-color: #e9c46a">#e9c46a</b>
<b style="background-color: #f4a261">#f4a261</b>
<b style="background-color: #e76f51">#e76f51</b>, no gradients. 

Optionally, you can use a black or white background.

---
## 4. (8♥)

Draw a line, pick a new color, move a bit

---
## 5. (8♥)

Replicate a natural concept (e.g. gravity, flocking, path following).

---
## 6. (8♥)

Generate some rules, then follow them by hand on paper.

---
## 7. (8♥)

Draw a line. Wrong answers only.

---
## 8. (8♥)

Circles only

---
## 9. (7♥)

Let someone else decide the general rules of your piece.

---
## 10. (7♥)

Interference patterns.

---
## 11. (7♥)

Curve only.

---
## 12. (7♥)

Do not repeat.

---
## 13. (7♥)

500 lines

---
## 14. (7♥)

```
// TRIPLE NESTED LOOP
```

---
## 15. (7♥)

Any shape, none can touch

---
## 16. (7♥)

Use something other than a computer as an autonomous process. (Or a non-computer random source)

---
## 17. (7♥)

Use sound.

---
## 18. (6♥)

```
10 SEARCH FOR "ENO'S OBLIQUE STRATEGIES"
20 OBTAIN ONE
30 THAT IS YOUR PROMPT FOR TODAY
```

---
## 19. (6♥)

Gradients without lines

---
## 20. (6♥)

```
// SUBDIVISION
```

---
## 21. (6♥)

Triangle subdivision.

---
## 22. (5♥)

Do some code golf! How little code can you write to make something interesting? Share the sketch and its code together if you can.

---
## 23. (5♥)

Use an API (e.g. the weather).

---
## 24. (5♥)

Small areas of symmetry.

---
## 25. (5♥)

One process grows, another process prunes.

---
## 26. (5♥)

Make a grid of all the permutations of something

---
## 27. (5♥)

2D Perspective.

---
## 28. (4♥)

Make something human.

---
## 29. (4♥)

```
function f(x) { 
    DRAW(x); 
    f(1 * x / 4); 
    f(2 * x / 4); 
    f(3 * x / 4); 
}
```

---
## 30. (4♥)

https://www.wolframalpha.com/input/?i=rule+30

---
## 31. (4♥)

```
// TREE
```

---
## 32. (4♥)

Monochrome gradient without lines

---
## 33. (4♥)

Use two colors only

---
## 34. (4♥)

Transform (e.g. shapes, text, information).

---
## 35. (3♥)

<span title="If you say &quot;I know technically not an insect but&quot;, you can also use spiders, shrimp, worms, insect-like mammals or birds.">Insects</span>; Algorithms, aesthetics, behaviour, simulation, simulacra.

---
## 36. (3♥)

Make a sketch using texture (image, collage).

---
## 37. (3♥)

Reverse the polarity.

---
## 38. (3♥)

Use continuous-valued noise (e.g. Perlin noise, Simplex noise, etc).

---
## 39. (3♥)

Text as primitive shape

---
## 40. (2♥)

This one is roughly based on the October challenge from [symbiocene.art](https://symbiocene.art).

```
// uppercase INPUT can be your own variables or expression
// INPUT_A is generally between 0.0 and 1.0
x += (INPUT_X - x) * INPUT_A;
y += (INPUT_Y - y) * INPUT_A;
```

---
## 41. (2♥)

Do it with a Fourier.

---
## 42. (2♥)

```
.5 + .5 * 5 ** .5
```

---
## 43. (2♥)

Make something that an alien would say "pfffft, my 3-year-old could do that".

---
## 44. (2♥)

Use OOP

---
## 45. (2♥)

[What are complex systems?](https://cssociety.org/about-us/what-are-cs#:~:text=Complex%20systems%20are%20systems%20where,from%20properties%20of%20the%20parts)

---
## 46. (2♥)

Place shapes. Alter the ones that overlap. Repeat.

---
## 47. (1♥)

```
for successive values of T:
    Y = X XOR T
```

---
## SOURCE CODE

```
from random import shuffle
prompts = open('prompts-unsorted.md').read().split('---')[1:-1]
def votes(p):
    return int(p.split('(')[1].split(')')[0])
def text(p):
    return p.split(')', 1)[1].strip()
shuffle(prompts) # removes order bias
prompts.sort(key=votes, reverse=True)
results = open('prompts-sorted.md', 'w')
ez_quine = '\n---\n## SOURCE CODE\n\n```\n%s\n```\n' % In[-1]
results.write('\n---\n'.join('## %i. (%i♥)\n\n%s\n' % (i+1,votes(p),text(p)) for (i,p) in enumerate(prompts)) + ez_quine)
results.close()
selection = open('prompts.md', 'w')
prompts31 = prompts[:31]
shuffle(prompts31)
selection.write('\n---\n'.join('## JAN.%i\n\n%s\n' % (i+1,text(p)) for (i,p) in enumerate(prompts31)))
selection.close()
```
