# Why Elm?
.float-right.shrink[![elm seattle logo](images/ElmSeattle.png)]
.slide-bottom[
Ivan Storck

October 2015

http://why-elm.elmseattle.org
]
---

class: center, middle, double-line-height
# Welcome, and Thanks Sponsors!

### 🎓 🏢 Code Fellows
### 🌎 Aerobatic
### 🍻 🍲 Seattle Startup Week

❤️ Special thanks to Pete Vilter and Evan Czaplicki
---

class: left
background-image: url(images/ivan-code-fellows-teaching.jpg)
.translucent.narrow[
Who I am and What I Do:

# Web Developer, Teacher and Entrepreneur

Based on my experience and talents,

I bridge the gap between Computer Science and industry.

I stand for:
- Excellence and Craftsmanship
- Usability and Accessibility
- Diversity and Inclusivity
- Sustainable Lifestyle
]
---
background-image: url(images/SarahJS.png)

# JavaScript (according to Sarah Connor)

---
# JavaScript
.red[
## `Undefined is not a function`
]

Tony Hoare said null was his *Billion Dollar Mistake*

Why are we still using it and seeing it every day?

### HTML5 and CSS are a bit of a mess, too

How do you center an image on the page?

.red[
## Why  do we have to learn 3 languages?
]
---

# Build tools are here to stay
Grunt, Gulp, Brunch, Make, Rake, Jake, *ad nauseum*

CoffeeScript — pioneered the way, and is still active

Babel — you're compiling to JS anyway

React — you're mixing in HTML, CSS, anyway

.red[
##*Why not design something nice from the beginning?*
]

What would that look like?

---
# Elm is&hellip;

- The best of functional programming in your browser
- Usable — Targeted towards JavaScript developers
- Inclusive — Evan Czaplicki: "Let's be mainstream"
- Reliable – No runtime exceptions - compilation finds errors
- Fast — Faster than React
- Inspiring — Angular 2.0, Brendan Eich

Example:

```elm
import Html exposing (span, text)
import Html.Attributes exposing (class)

main =
  span [class "welcome-message"] [text "Hello, World!"]
```
---

# Functional Programming is&hellip;
- Immutability - Values don't change unexpectedly
- Pure functions - predictable and testable outcomes
- Pattern Matching - clean code over complex if statements
- Declarative vs Imperative
- Scalable
- Reactive

???

Imperative - one instruction after another.
Declarative - describing what you want to have happen

You probably already know a great declarative programming language, SQL.
And CSS is declarative too.
---
# Don't fear the type system
It's not like Java

```elm
import Graphics.Element exposing (..)
import Mouse


main =
  Signal.map show Mouse.position
```

Catching type errors at compile time makes code more reliable (vs runtime)
---
# Example: Binary Tree
```elm
type Tree a = Empty | Node a (Tree a) (Tree a)
```

Imagine doing this in Java. One super class and two sub classes just to define a tree in the first place!

Imagine JS. It is not quite as bad at first,

but imagine trying to refactor the resulting code later if you need to change the core representation.

Sneaky breakages everywhere!
---
# Dev Environment and workflow
- Atom
```
apm install linter linter-elm-make language-elm
```
- Vim
  - https://github.com/ElmCast/elm-vim

- Elm Brunch
  - https://github.com/ivanoats/elm-brunch-starter
---
# Demonstration of Elm Brunch
---
# Other Elm Resources

- [Pragmatic Studio](https://pragmaticstudio.com/elm) video tutorials
- [Elm Discuss](https://groups.google.com/forum/?fromgroups#!forum/elm-discuss) mailing list
- [#elm](seattlehacks.herokuapp.com) channel on seattlehacks Slack
- [Elmcasts.io](http://elmcasts.io)

People to follow:
- [Evan Czaplicki](https://twitter.com/evancz)
- [Richard Feldman](https://twitter.com/rtfeldman)
- [Yan Cui](https://twitter.com/theburningmonk)
- [Pete Vilter](https://twitter.com/)
- [Ivan Storck](https://twitter.com/ivanoats)

Organizations:
- [Elm](https://twitter.com/elmlang)
- [ElmSeattle](https://twitter.com/elmseattle)
