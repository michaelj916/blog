---
layout: post
title:  "First blog post! (testing)"
date:   2022-02-16 13:48:06 -0800
categories: jekyll update
---
# Welcome!

This is officially my first blog post. I won't talk about anything too fancy here, but just to test what Jekyll can do I would like to share some snippets of code that talk about a list of numbers I am particularly fond of.

The fibonacci sequence is an infinite sequence that can be defined recursively as: `F(n) = F(n - 1) + F(n - 2)`. *Recursive* means that the definition of the function includes itself, and we will explore recursion in future blog posts when exploring the Mandelbrot set and other fractals. 

<!--
Here are a few examples of the fibonacci sequence in math and nature:

![golden-spiral](/assets/golden-spiral.jpg)
-->

Here is a quick and simple way to gather *n* fibonacci numbers in the functional programming language Haskell:
{% highlight Haskell %}
main = do
    print $ take 50 fibs

fibs = map fst $ iterate (\(a, b) -> (b, a+b))(0,1)    
{% endhighlight %}
With this, we have created an infinite list of fibonacci numbers, `fibs`, and we are simply printing out a list of *that* list's first 50 elements (i.e. the first 50 fibonacci digits). Haskell is really neat beacuse we can use the Prelude libraries functions to do so many things which normally would require loops or if-then statements. This is not really an example of functional programming, but I am quite fond of Haskell at the moment so I will include it here.

This wraps up my first blog post, I am looking forward to creating more. Thank you for your time.
