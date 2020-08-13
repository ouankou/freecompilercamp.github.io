---
layout: exam
title: "Practical for Working with Complex Types"
author: "@vec4"
date: 2020-06-23
categories: practical
exam_name: complex-types
exam_language: c++
tags: [rose, practical]
image: freecompilercamp/pwc:rose-exam
---

## Check Your Understanding ##
This purpose of this test is to evaluate your understanding of working with complex types with ROSE.

This is a "closed-book" test and the terminal has been removed. Write your code in the text editor and click the "Submit Code" button to have the server evaluate your submission. You will be made aware of any compilation errors, but test cases will not be made available.

### Task ###
Implement a ROSE translator that traverses the AST for `const` type-qualified variables *that are function parameters*. Print only each variable name to the standard output.

Example input:

<figure class="lineno-container">
{% highlight cpp linenos %}
const int foo = 3;

void bar(const float y) {
  const int x = 54;
  return x*y;
}

int main(int argc, char* argv[]) {
	return 0;
}
{% endhighlight %}
</figure>

In this example, there is only one `const` type-qualified function parameter: `y`.
