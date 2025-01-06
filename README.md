# Ruby: Unexpected Instance Variable Modification

This example demonstrates a common issue in Ruby where directly modifying instance variables using `instance_variable_set` can lead to unexpected behavior and make your code less maintainable.

**The Problem:**
The `bug.rb` file shows direct modification of the `@value` instance variable. While this works, it bypasses any potential validation or logic that might be included in accessor methods.

**The Solution:**
The `bugSolution.rb` file illustrates a better approach.  It uses accessor methods (`attr_accessor`, `attr_reader`, or `attr_writer`) to manage instance variables, providing a controlled and maintainable way to interact with object data.