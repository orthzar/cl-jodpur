# cl-jodpur, an implementation of JODPUR in Common Lisp

>"Supporting every statement is an asterisk. Supporting each asterisk is two more asterisks. It's asterisks all the way down." -- some guy, who thinks he's clever, but who is actually an idiot

## Marketing Introduction

Are you looking for the new rizz in programming languages? Well, look no further!

JODPUR...
- is the only programming language you could ever need
- secures your data via ChatGPT
- is NIST-approved for use in space
- has all the best practices
- is not named after a musical note
- types "safe"
- uses TOML recreationally, but only in the privacy of it's own home
- relies upon robustness
- believes everything might be an object
- pronounces "h" properly
- This just in, NIST has revoked JODPUR's use-in-space approval, so put away the champaign and get your shoes back on.
- is intended to be as simple as programming in assembly
- considers "F's in chat" to be a slur
- rejects internationalization because every country is actually a part of Texas
- is durable against all of your purposes
- rejects your real estate and substitutes it's own
- is not dating anyone right now but might be in the future
- has received federal funding for an unrelated project concerning Mozambique
- enjoys a good logger
- is afraid to hear what everyone is thinking
- oozes flexibility
- was written on an afternoon
- believes that Mars will not be colonized by humanity for at least a thousand years
- is available on every streaming platform
- supplies all your chain-attacks
- is currently under felony indictment in West Dakota for jaywalking
- earned it's bachelor's of arts in computer science at Downton Abbey
- is probably parsable by a ton of programs
- was once fired for making appropriate jokes about management
- doesn't remotely work
- thinks that it's bad they ejected Pluto, the dog, from the solar system
- is insecure                 about it's appearance
- believes that all software was made fully-formed, bugs and all, last thursday
- has spent an exorbitant amount of time on the toilet thinking about how to destroy the toilet industry
- was the recipient of an award from the KKK but rejected it because it would be "too great a strain on it's innate modesty". (it it it it it)
- hasn't seen it's feet in years
- is on a TOML-fueled vision quest to find it's wallet
- has never said anything of the sort
- is often called a crypto-soviet which is confusing because the correct nomenclature is crypto-oblast
- has endured a century of ridicule at the hands of numaticists
- persists in asserting that the sun is a flat disk and that eclipses are actually epi-rotations of the sun
- makes people nostalgic for their most recent root canal

## Serious Introduction (to a joke programming language)

**WARNING: This entire repo is not remotely usable yet. This README is a goal, not a reflection of the current status of the repo (see [this](https://tom.preston-werner.com/2010/08/23/readme-driven-development.html) for an explanation).**

JODPUR stands for ```Joe's Own Descriptive Programming langUage Rodeo```.

This is an initial implementation of JODPUR, a joke programming language whose syntax is TOML. The joke here is that JODPUR uses TOML for syntax; everything else is not intended to be a joke (well, to me, anyways. You are free, for the time being, to view JODPUR as a top-to-bottom joke.).

cl-jodpur is not a reference implementation. Refer to JODPUR-specification.toml if you want to implement JODPUR yourself, or to just experience the joke first-hand.

cl-jodpur compiles to Common Lisp.

cl-jodpur is intended to be portable across Common Lisp implementations, but I will probably only test it using SBCL.

cl-jodpur uses cl-toml to parse/generate JODPUR syntax (yes, this means that JODPUR is homoiconic).

Inside the body attribute of a JODPUR function, you can either put host language code as a string (e.g. ```"(+ n n)"``` or ```"n + n;"```) or you can use a Smalltalk-like message-passing semantic (e.g. ```[i, :=, k]```). (I said the use of TOML as syntax was the joke, and I hope you can see now the fruition of that joke. But wait, there is more fruit to experience.)

## Dependencies

You will need the following to run cl-jodpur:
- SBCL
- cl-toml (which is available via QuickLisp (which is available in the Debian and Ubuntu repos))
- More time than sense.

## Installation

```
git clone https://github.com/orthzar/cl-jodpur/
sbcl --load "cl-jodpur.lisp"
```

## Usage

In SBCL, run this Lisp form:
```
(start-jodpur-prompt)
```

It will start a JODPUR command prompt, which begins with a ```J ```.

To define a JODPUR function object:
```
J [funkifier]
type = function
arguments = [ your-name ]
body = [
        [concatenate, "Bro, ", your-name, " is so funky fresh."]
       ]
side-effects = [ terminal-out ]
```

Call ```funkifier``` like this:
```
J [ funkifier, "Bob Sacamano" ]
```

To exit the cl-jodpur prompt, run this JODPUR command:
```
J exit
```
(That will drop you into SBCL's prompt, which you can exit by evaluating ```(exit)```).

## FAQ (Fans (yes, JODPUR has fans) Ask Questions)

- Q: Why should I use this?
  - A: Because I told you so.
- Q: Is this dedicated to anyone?
  - A: This is dedicated to whomever happens to read this and enjoy the jokes.
- Q: Are you taking questions at this time?
  - A: No.
- Q: Are types transitive?
  - A: I don't know. Is your type inferencer capable of distinguishing between a garden hose and a monad?
- Q: Was this written by ChatGPT?
  - A: It was a dark and stormy night. Joe was at home typing furiously to get the readme for his favorite new language finished before the deadline. If his boss had told him once he had told him a thousand times: you have to finish the readme for your joke programming language by the deadline. His boss barged in and demanded to see what he was typing. Joe didn't want his boss to know that he was almost done.

## TODO

- [ ] Make this work, like for real. (see this joke has layers: layer one is the bit about TOML, and layer two is that I intend to make this usable.)
- [ ] rlwrap support.
- [ ] Figure out namespaces and packages.
- [ ] Get someone to make a logo of half of a pair of jodpurs.
- [ ] Make a needlessly marketing-focused website.
- [ ] Write the website in cl-jodpur. (I will be so angry if this proves to be easier than it has any right to be.)
- [ ] Add said logo to said website and to this repo.
- [ ] Pester some people on #lisp to use cl-JODPUR.
- [ ] ???
- [ ] Profit.

