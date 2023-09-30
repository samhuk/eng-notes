A bit about me and my thoughts and views on software and engineering:

* Thoughts and views can change and be changed.
* Make something that earns people money, saves them time, simplifies a workflow, or something that is required for compliance.
* Have care and craftsmanship.
* Correctly prioritize features
  * How long features take to complete often follow a [Pareto distribution](https://en.wikipedia.org/wiki/Pareto_distribution).
  * *"~80% of features take ~20% of the time"*
  * Focus on the 80%, with the 20% in mind for later.
* My process:
  1. Get requirement(s)/problem(s).
  2. Make sure they are the correct ones to solve. GOTO 1 until correct.
  3. Has somebody already created a solution or similar?
  4. If so, use as base. GOTO 6.
  5. Else, figure out solution. Research. Break the problem down. Need help?
  6. Iterate whilst liasing with stackholders. Ensure on right track. Need initial buy-in?
  8. Iterate through releases. alpha -> beta, 0 -> 1 -> 2. Plan path to GA.
  9. Market, maintain, extend, semver, care, profit!
* Don't be religious.
  * Optimal decisions almost always sit between 0.2 and 0.8 of a decision space, almost never at the extremes.
  * Example: Optimal amount of tech debt is never at 0% or 100%. Tech debt is like fiat debt. None or lots can be bad.
* Many problems are made much easier by focusing on:
  * A simpler/toy problem first
  * The required behaviors
  * The required data structures and APIs/interfaces
  * The data life-times
  * The involved data ETL processes.
  * Etc.
* Prefer composition (excluding game dev).
  * Inheritence often leads to complicated code. *Sometimes* is right path, but unlikely.
  * Composition promotes divide & conquer problem solving and composible architectures.
* PEP20 (Zen of Python).
  * Numbered list: https://python.land/the-zen-of-python.
  * My favourites:
    * 2 - Because implicit code is expressive to no-one but the creator.
    * 5 - Because flat lists of operations are more readable and composable versus deep stacks and promote problem solving by divide and conquer.
    * 12 - Because decisions without data are guesses
    * 13 - Because Go did this and it went well
    * 17 - Because if you haven't got an elevator pitch for something you are doing, you probably don't understand it.
* Follow the KISS principle (but sometimes "big" problems need "big" solutions).
* Follow the SR principle.
* Follow *"LDD"*
  * Library-Driven Development.
  * *"Imagine the code you are writing, whatever it is for, is a 'package'."*.
  * This mindset promotes creating reusable code with room for reinterpretation.
* Be cautious of TDD
  * Theoretically great in pre-defined toy scenarios, but practically not that useful.
  * Create tests, but don't religiously create all tests before all of your functional code.
* Be cautious of SOLID
  * Needs to be reframed and moderated by business and common sense in order to be useful.
* Why engineering can sometimes fail:
  * Non-technical leaders
  * Acceptance of deviance
  * Private Equity financing
