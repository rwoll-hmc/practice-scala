Some Initial Scala Thoughts
===========================

Scala is by far the most unique language I've used. Its fusion of Object-Oriented
and Functional paradigms are both a beautiful and confusing partnership. For
instance, in a functional language, like Haskell or SML, I default to thinking
in folds and recursion when I want to use a *for* or *while* loop, and in the Java
Programming Language (with newer features aside) I default to thinking in *for* and
*while* loops; in Scala, I was never certain what to reach for (no pun intended).
In solving the Rainfall problem, I wanted to use a for loop with a break statement,
but this turned out to be fairly difficult to write in Scala, and I instead encountered
the `takeWhile`&mdash;essentially a wrapper for this behavior.

Scala's flexible formatting options (e.g. being able to write `list.filter(myPred)` as
`list filter myPred`) makes for a very inconsistent look and feel to the code.
With time, I'm assuming I will gain more insight into the Scala-style of doing
things by following the style guide more closely and this flexibility will become
only an advantage. However, I think the compiler should be stricter; for example,
when writing two synonymous things like `List()` and `Nil` in a `case` statement,
it should only let you do the more stylistic one `Nil`, unless there is some need
to differentiate the types. (Some such cases exist as we saw in the assignment.)

On another note, the documentation for Scala, like Java docs, is very comprehensive
for the built in APIs. This is esential for writing Scala code, and I appreciated
how easy it was to find and use&mdash;the examples are an added bonus.

While I think semicolonless code looks less cluttered, I think Scala requiring
them (instead of inferring them), would make it easier to read for new people.
Figuring out indentation and the `|` character I think are unintuitive and harder
to read than the alternative.

One feature that I really enjoyed in Scala, is its pattern matching capabilities
which is also one of my favorite patterns in Haskell. It is a nice way to simplify
otherwise complicated conditionals and destructuring code. Scalas support for
lambdas and higher-order functions is also amongs its strong arguments. Being
able to do partial application and pass functions around but also use objects
seems to be a plus.
