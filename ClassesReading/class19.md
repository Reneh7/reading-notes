# Class nineteen Reading

## Can you change the state of a data structure using functional programming?

Functional programming emphasizes immutability, meaning that once data is created, it should not be modified. Instead of changing the state of a data structure, functional programming encourages creating new data structures by applying functions to existing ones. This approach ensures that data remains consistent and predictable, as operations don't have side effects on the original data. While it's possible to simulate state changes by creating new data structures with the desired modifications, true state mutation is discouraged in functional programming to maintain the principles of purity and immutability, which contribute to code that is easier to reason about and test.

## Define purely functional programming

Purely functional programming is a programming paradigm haracterized by the use of pure functions, which are deterministic, free from side effects, and immutable. In this paradigm, data is not modified in place; instead, new data structures are created through functional transformations.

## How do you think purely functional programming will differ from the programs you’ve written so far in this course?

Purely functional programming, in contrast to the programs I've written in this course, revolves around the concept of immutability and the avoidance of side effects. It enforces the principle that data structures once created cannot be modified; instead, new structures are generated through transformations, enhancing code safety and predictability. This approach relies heavily on higher-order functions, recursion, and pattern matching, resulting in more concise and modular code. Unlike the imperative paradigm I've used in my coursework, purely functional programming minimizes mutable state and isolates side effects, making code more robust, maintainable, and less prone to bugs associated with state changes and unpredictable side effects.
