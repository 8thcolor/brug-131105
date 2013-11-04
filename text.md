text.md

# Ruby, tests, code review and automation.

Hi everybody, nice to be here today. Quite new to the Ruby community, but so
great to feel as a member of.

I'm Christophe, I'm a developer with various experiences such as academic
research in AI/teaching/sysadmin for a French online video game/C++ dev
developing simulation of spread of disease ...

and 2 years ago I've founded 8th Color with Martin, where we're developing tool
for devs with the idea that Better Developers make Better Software.

We've recently launched our first Ruby app: PullReview, an automated code review.

But let's put that aside and start.

---

## Ruby is Dynamic typing

Let's start first with a recap about Ruby:

When we talk about dynamic typing, we talk about a mechanism where the type of a
variable can change and be resolved on the fly at the exact moment it gets
parsed by the interpreter.

When we talk about static typing, we talk about a mechanism where the type of a
variable is resolved in advance by the interpreter/compiler

---

## and strong typing

It’s not because Ruby lets you change the type of an object as many
times as you want that it doesn’t care about what you do with it. If you start
mixing several types together in an expression, it won’t try to understand what
it means, nah… that is too complicated. Instead, ruby will throw an exception…
end of story. This is why we say that Ruby is a strongly typed language.

"strongly typed" in the sense that typing errors are prevented at runtime and
they do little implicit type conversion, but these languages

In fact, it's what leads to duck typing

---

## Ruby is Duck typing

duck typing is a style of typing in which an object's methods and properties
determine the valid semantics, rather than its inheritance from a particular
class or implementation of a specific interface.

> When I see a bird that walks like a duck and swims like a duck and quacks like
> a duck, I call that bird a duck.

otherwise, at the moment you respect the contract i.e. it offers the expected
prototypes of method, that's ok.

---

## Getting Weak Typing with Duck Typing

The fact is, that ruby is so dynamic (and I use the term not in its official
context) in nature, that strong typing loses much of its punch. Granted, the
default operators will act in a strongly typed manner, but if you took the time
to override these operators on the basic primitives (which are really
objects/classes), you’d end up with something that looked pretty weakly typed.

And you get the best of both worlds.

## Refs

* http://www.rubyfleebie.com/ruby-is-dynamically-and-strongly-typed/
* http://www.dreamincode.net/forums/topic/179748-dynamic-typing/
* https://en.wikipedia.org/wiki/Ruby_%28programming_language%29
* https://en.wikipedia.org/wiki/Dynamic_typing#Dynamic_type-checking_and_runtime_type_information
* http://c2.com/cgi/wiki?DavidThomasOnTheBenefitsOfDynamicTyping
* http://stackoverflow.com/questions/520228/is-ruby-strongly-or-weakly-typed
* https://en.wikipedia.org/wiki/Duck_typing#In_Ruby
* http://en.wikipedia.org/wiki/Test-driven_development
* http://programmers.stackexchange.com/questions/71654/code-reviews-what-are-the-advantages
* http://www.slideshare.net/gvwilson/bits-of-evidence-2338367
* http://programmers.stackexchange.com/questions/15874/tips-on-persuading-boss-that-code-review-is-a-good-thing
* http://www.devart.com/review-assistant/learnmore/benefits.html
* http://stackoverflow.com/questions/125367/dynamic-type-languages-versus-static-type-languages
* http://programmers.stackexchange.com/questions/141485/what-is-the-difference-between-static-code-analysis-and-code-review
* http://www.nickokiss.com/2009/01/code-reviews-manual-or-automated.html
* http://stackoverflow.com/questions/322807/which-software-development-practices-provide-the-highest-roi
* http://sd.jtimothyking.com/2006/07/11/twelve-benefits-of-writing-unit-tests-first/
* http://dipperstove.com/development/software-testing-benefits.html
* http://tech.myemma.com/experiences-test-driven-development/
* http://stackoverflow.com/questions/322807/which-software-development-practices-provide-the-highest-roi
