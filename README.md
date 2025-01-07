# CSS Float Layout Bug

This repository demonstrates a common issue encountered when using floats in CSS: unexpected collapsing of floated elements when their total width exceeds the parent container's width.  The `bug.css` file contains the problematic code, while `bugSolution.css` provides a solution.

## Problem

The problem stems from the use of `float: left;` on divs without proper clearing of floats. When the sum of the widths of the floated elements is greater than their parent's width, some browsers may unexpectedly collapse or shrink the elements, leading to an inconsistent layout.

## Solution

The solution involves adding a clearfix (or using other appropriate techniques) to ensure that the parent container correctly accounts for the width of the floated elements.  The `bugSolution.css` file illustrates this approach.