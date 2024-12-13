# Tailwind CSS Configuration Error

This repository demonstrates a common issue encountered when configuring Tailwind CSS: the inability to have custom styles picked up from components due to an incorrect or incomplete configuration of the `content` option in `tailwind.config.js`.

## Problem

When building components with Tailwind classes, those classes are not being applied.  The problem lies in how Tailwind scans for CSS utility classes within your project files.

## Solution

The solution involves carefully reviewing and correcting the `content` array in `tailwind.config.js` to accurately reflect the location and types of files containing your Tailwind classes.

## How to Reproduce

1. Clone this repository.
2. Follow the instructions in `bug.js` to set up a basic Tailwind CSS project with a misconfigured `content` path.
3. Attempt to use custom Tailwind classes within a component. Notice they won't be applied.
4. Examine the corrected `content` path in `bugSolution.js`. Run `npm run build` or a similar command to build your project. Observe that the classes are now applied correctly.