## 8. Traveling Wave Functions: Identifying Valid Mathematical Models

For a mathematical equation to accurately describe a physical traveling wave, it must represent a shape that moves through space over time *without* changing its fundamental form. 



### Step 1: The Core Rule for Traveling Waves
To maintain its shape as it travels at a constant velocity ($v$), the spatial variable ($x$) and the time variable ($t$) must be locked together in a specific, linear relationship. 

Any true traveling wave function $f(x,t)$ must be able to be written in the form:
$$f(x \pm vt)$$

* **$(x - vt)$:** Represents a wave traveling to the **right** (positive x-direction).
* **$(x + vt)$:** Represents a wave traveling to the **left** (negative x-direction).

If the inside of the function cannot be simplified or factored into this exact linear relationship, it is **not** a valid traveling wave. Let's test three different mathematical functions to see if they pass.

---

### Step 2: Evaluating Function A
**The Function:** $$f(x,t) = A \cos(kx^2 - \omega t)$$

**The Verdict: NO.**
**Why?** Look closely at the spatial variable $x$; it is squared ($x^2$). Because of this non-linear term, there is no mathematical way to factor the inner argument into the required $(x \pm vt)$ form. Physically, this equation describes a ripple that would distort and change its shape as time goes on, violating the definition of a stable traveling wave.

---

### Step 3: Evaluating Function B
**The Function:** $$f(x,t) = A(x - vt)^2$$

**The Verdict: YES.**
**Why?** This function directly groups $x$ and $t$ exactly as $(x - vt)$. Even though the entire group is squared on the outside, the internal relationship between position and time is preserved perfectly. It represents a valid traveling wave pulse moving to the right at a constant speed $v$.

---

### Step 4: Evaluating Function C
**The Function:** $$f(x,t) = A \log(x + vt)$$

**The Verdict: YES.**
**Why?** Similar to Function B, the variables $x$ and $t$ are grouped in the exact linear form required: $(x + vt)$. The fact that this group is placed inside a logarithmic function does not break the core relationship. It represents a valid traveling wave moving to the left at a constant speed $v$.

### Conclusion for Presentation
The key takeaway is that the *outer* function—whether it is a cosine, a square, or a logarithm—simply determines the physical *shape* of the wave. However, it is the *inner* argument—the strict linear pairing of $(x \pm vt)$—that guarantees that shape will properly travel through space without falling apart.