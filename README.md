### Summary

A bit about me and my thoughts and views on software and engineering.

This is a live document; thoughts and views can change and be changed.

### Mantra

**Make to delight, care about your work, make the world a better place, and do no evil.**

### General Takes

* If stuck for ideas, make something that earns people money, saves them time, simplifies a workflow, or something that is required for compliance.
* Optimize the process, then work in the optimized process. However, compromise when appropriate.
* Correctly prioritize features
  * How long features take to complete often follow a [Pareto distribution](https://en.wikipedia.org/wiki/Pareto_distribution).
  * *"~80% of features take ~20% of the time"*
  * Focus on the 80%, with the 20% in mind for later.
* My process:
  | **i** | **task**                                                                           |
  |----|---------------------------------------------------------------------------------------|
  | 0  | Get requirement(s)/problem(s).                                                        |
  | 1  | Make sure they are the correct ones to solve. GOTO 0 until correct.                   |
  | 2  | Has somebody already created a solution or similar? If so, GOTO 4                     |
  | 3  | Figure out solution. Research. Break the problem down. What are the behaviors? Need help? |
  | 4  | Iterate whilst liasing with stakeholders. Ensure on right track. Need initial buy-in? |
  | 5  | Iterate through releases. alpha -> beta, 0 -> 1 -> 2. Plan path to GA.                |
  | 6  | Market, maintain, extend, semver, care, profit!                                       |
* Don't be religious.
  * Optimal decisions almost always sit between 0.2 and 0.8 of a decision space, almost never at the extremes.
  * Example: Optimal amount of tech debt is never at 0% or 100%. Tech debt is like fiat debt. None or lots can be bad.
* 1000 LoC that clearly expresses intent is better than 100 equiavelent LoC that expresses nothing. See ZoP PEP2.
* Many problems are made much easier by focusing on:
  * A simpler/toy problem first
  * The required behaviors
  * The required data structures and APIs/interfaces
  * The involved data ETL processes.
  * Etc.
* Follow *"LDD"*
  * Library-Driven Development.
  * *"Imagine the code you are writing, whatever it is for, is a 'package'."*.
  * This mindset promotes creating reusable code with room for reinterpretation.

### Takes on Some Well-known Principles

* Prefer composition (excluding game dev).
  * Inheritence often leads to complicated code. *Sometimes* is right path, but unlikely.
  * Composition promotes divide & conquer problem solving and composible architectures.
* Follow the KISS principle (but sometimes "big" problems need "big" solutions).
* Follow the SR principle.
* Follow PEP20 (Zen of Python, https://python.land/the-zen-of-python).
  * My highlights:
    * 2 - Because implicit code is expressive to no-one but the creator.
    * 5 - Because flat lists of operations are more readable and composable versus deep stacks and promote problem solving by divide and conquer.
    * 12 - Because decisions without data are guesses
    * 13 - Because Go did this and it went well
    * 17 - Because if you haven't got an elevator pitch for something you are doing, you probably don't understand it.
* Be cautious of TDD
  * Theoretically great in pre-defined toy scenarios, but practically not that useful.
  * Create tests, but don't religiously create all tests before all of your functional code.
* Be cautious of SOLID
  * Needs to be reframed and moderated by business and common sense in order to be useful.
 
### Cautions

* Why engineering can sometimes fail:
  * Non-technical leaders
  * Acceptance of deviance
  * Private Equity financing
