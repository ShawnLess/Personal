---
layout: distill
title: Fundametal Math for Machine Learning
description: Basic math knowledge and conceptions for machine learning.
tags: Math ML
giscus_comments: true
date: 2025-1-27
featured: true
# mermaid:
#  enabled: true
#  zoomable: true
# code_diff: true
# map: true
# chart:
#  chartjs: true
#  echarts: true
#  vega_lite: true
# tikzjax: true
# typograms: true

# authors:
#  - name: Albert Einstein
#    url: "https://en.wikipedia.org/wiki/Albert_Einstein"
#    affiliations:
#      name: IAS, Princeton


# bibliography: 2018-12-22-distill.bib

# Optionally, you can add a table of contents to your post.
# NOTES:
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
#   - we may want to automate TOC generation in the future using
#     jekyll-toc plugin (https://github.com/toshimaru/jekyll-toc).
toc:
  - name: Linear Regression
    # if a section has subsections, you can add them as follows:
    # subsections:
    #   - name: Example Child Subsection 1
    #   - name: Example Child Subsection 2
  - name: Logistic Regression


# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
# _styles: >
#  .fake-img {
#    background: #bbb;
#    border: 1px solid rgba(0, 0, 0, 0.1);
#    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
#    margin-bottom: 12px;
#  }
#  .fake-img p {
#    font-family: monospace;
#    color: white;
#    text-align: left;
#    margin: 12px 0;
#    text-align: center;
#    font-size: 16px;
#  }
---

## Linear Regression

This theme supports rendering beautiful math in inline and display modes using [MathJax 3](https://www.mathjax.org/) engine.
You just need to surround your math expression with `$$`, like `$$ E = mc^2 $$`.
If you leave it inside a paragraph, it will produce an inline expression, just like $$ E = mc^2 $$.

In fact, you can also use a single dollar sign `$` to create inline formulas, such as `$ E = mc^2 $`, which will render as $ E = mc^2 $. This approach provides the same effect during TeX-based compilation, but visually it appears slightly less bold compared to double-dollar signs `$$`, making it blend more naturally with surrounding text.

To use display mode, again surround your expression with `$$` and place it as a separate paragraph.
Here is an example:

$$
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
$$

Note that MathJax 3 is [a major re-write of MathJax](https://docs.mathjax.org/en/latest/upgrading/whats-new-3.0.html) that brought a significant improvement to the loading and rendering speed, which is now [on par with KaTeX](http://www.intmath.com/cg5/katex-mathjax-comparison.php).

---


