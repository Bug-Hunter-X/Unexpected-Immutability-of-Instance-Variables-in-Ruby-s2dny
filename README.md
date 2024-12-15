# Unexpected Immutability of Instance Variables in Ruby

This repository demonstrates a common, yet subtle, error in Ruby: the unexpected immutability of instance variables when a setter method is not explicitly defined.

## The Bug

In Ruby, if you try to modify an instance variable directly from outside the class definition, it won't work unless you define an appropriate setter method.  The `bug.rb` file shows this unexpected behavior. Attempting to change the instance variable `@value` does not change the instance variable's value.

## The Solution

The `bugSolution.rb` file demonstrates the proper way to address this: define a setter method. This allows controlled modification of the instance variable from outside the class.

## How to Reproduce

1. Clone this repository.
2. Run `bug.rb` using Ruby. Note the unexpected output.
3. Run `bugSolution.rb` using Ruby. Note that the output now reflects the changes.

This example highlights the importance of understanding Ruby's approach to instance variable access and the need for explicit setter methods when modification is required.