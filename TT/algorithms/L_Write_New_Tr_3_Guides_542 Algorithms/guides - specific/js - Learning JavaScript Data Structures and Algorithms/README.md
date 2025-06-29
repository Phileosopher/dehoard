Learning JavaScript Data Structures and Algorithms

[GitHub - loiane/javascript-datastructures-algorithms: collection of JavaScript and TypeScript data structures and algorithms for education purposes. Source code bundle of JavaScript algorithms and data structures book](https://github.com/loiane/javascript-datastructures-algorithms)

[![Build Status](https://travis-ci.org/loiane/javascript-datastructures-algorithms.svg?branch=third-edition)](https://travis-ci.org/loiane/javascript-datastructures-algorithms)
[![codecov](https://codecov.io/gh/loiane/javascript-datastructures-algorithms/branch/master/graph/badge.svg)](https://codecov.io/gh/loiane/javascript-datastructures-algorithms)
[![devDependencies Status](https://david-dm.org/loiane/javascript-datastructures-algorithms/dev-status.svg)](https://david-dm.org/loiane/javascript-datastructures-algorithms?type=dev)
[![dependencies Status](https://david-dm.org/loiane/javascript-datastructures-algorithms/status.svg)](https://david-dm.org/loiane/javascript-datastructures-algorithms)
[![Greenkeeper badge](https://badges.greenkeeper.io/loiane/javascript-datastructures-algorithms.svg)](https://greenkeeper.io/)

Source code of Learning JavaScript Data Structures and Algorithms book, third edition.

## List of available chapters:

 01: [JavaScript: a quick overview](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter01)
 02: [ECMAScript and TypeScript Introduction](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter02)
 03: [Arrays](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter03)
 04: [Stacks](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter04)
 05: [Queues and Deques](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter05)
 06: [LinkedLists](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter06)
 07: [Sets](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter07)
 08: [Dictionaries and Hashes](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter08)
 09: [Recursion](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter09)
 10: [Trees](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter10)
 11: [Heap](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter11)
 12: [Graphs](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter12)
 13: [Sorting and Searching Algorithms](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter13)
 14: [Algorithm Design and Techniques](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter14)
 15: [Algorithm Complexity](https://github.com/loiane/javascript-datastructures-algorithms/tree/third-edition/examples/chapter15)

### Third Edition Updates

 Algorithms using ES2015+ (ES6+)
 New data structures and algorithms
 All chapters rewritten and reviewed
 Three (3) new chapters
 Creation of a Data Structures and Algorithms library that can be used in the browser or with Node.js
 Algorithms tested with Mocha + Chai (test code available in `test` directory)
 TypeScript version of the source code included (library and tests)

## Project Structure

`src/js/index.js` file contains all the data structures and algorithms listed by chapter.

```
|_examples (how to use each data structure and algorithm, organized by chapter)
|_src
|___js (source code: JavaScript version)
|_____data-structures
|_______models (classes used by DS: Node, ValuePair, ...)
|_____others (other algorithms such as palindome checker, hanoi tower)
|___ts (source code: TypeScript version)
|_____data-structures
|_______models
|_____others
|_test (unit tests with Mocha and Chai for src)
|___js (tests for JavaScript code)
|___ts (tests for TypeScript code)
```

## Installing and running the book examples With Node

 Install [Node](https://nodejs.org)
 Open terminal/cmd and change directoty to this project folder: `cd /Users/.../javascript-datastructures-algorithms` (Linux/Max) or `cd C:/.../javascript-datastructures-algorithms`
 run `npm install` to install all depencies
 To see the examples, run `http-server html` or `npm run serve`. Open your browser `https:\\localhost:8080` to see the book examples
 Or `cd html/chapter01` and run each javascript file with node: `node 02-Variables`

## Running the examples in the browser

 Right click on the html file you would like to see the examples, right click and 'Open with Chrome (or any other browser)'

 Or open the `examples/index.html` file to easily nagivate through all examples:

 Demo: [Data Structures and Algorithms with JavaScript](https://javascript-ds-algorithms-book.firebaseapp.com/)

<img src="examples/examples-screenshot.png">

Happy Coding!
