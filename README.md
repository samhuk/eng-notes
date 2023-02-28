A bit about me and my thoughts and views on software and engineering:

* **Thoughts and views can change and be changed.**
* **Make something that earns people money** or something they must have for compliance.
* **Have care and craftsmanship.**
* I'm not from a CS background, so my thinking is often more practical, less academic.
* **Correctly prioritize features**
  * Features for most projects follow a [Pareto distribution](https://en.wikipedia.org/wiki/Pareto_distribution).
  * *"~80% of features take ~20% of the time"*
  * Accordingly, the last 20% of features takes the remaining 80% of the time.
  * Focus on the 80%, with the 20% in mind.
* **My process**:
  1. Get requirement(s)/problem(s).
  2. Make sure they are the correct requirement(s)/problem(s) to solve.
  3. Has somebody already created a solution or similar? (Don't reinvent the wheel)
  4. If so, use as base. Adapt and move onto PoC/validation.
  5. Else, figure out solution. Break the problem down. Divide and conquer. Need help?
  6. Iterate and liase stackholders, ensure on right track. Need initial buy-in?
  8. Iterate through stages: alpha -> beta, 0 -> 1 -> 2, eventually to GA.
  9. Maintain, extend, semver, care, profit!
* **Don't be religious**.
  * Nothing is binary.
  * Optimal decisions almost always sit between 0 and 1, almost never at 0 and 1.
  * For example: Optimal amount of tech debt is never at 0% or 100%. Tech debt is just like fiat debt. None or lots *can* be a hinderance.
* Many problems are made much easier by focusing on:
  * Solving a simpler/toy problem first
  * Required behaviors
  * Required data structures
  * Data life-times
  * The involved ETL processes.
  * Etc.
* **Prefer composition** (except in game dev).
  * Inheritence often leads to complicated code. *Sometimes* is the right path, but less likely.
  * Composition promotes divide & conquer problem solving and composible architecture.
* **PEP20** (Zen of Python).
  * Numbered list: https://python.land/the-zen-of-python.
  * Some of my highlights:
    * 2 - Because implicit code is not expressive to anyone but the creator.
    * 5 - Because flat lists of operations are more readable and composable versus deep stacks and promote problem solving by divide and conquer.
    * 12 - Because decisions without data are guesses
    * 13 - Because Go did this and it went well
    * 17 - Because if you haven't got an elevator pitch for something you are doing in software, you don't understand it.
* **KISS principle** (but sometimes "big" problems need "big" solutions).
  * Don't overcomplicate the problem or solution.
* **SR principle**
* **"LDD"**
  * Library-Driven Development.
  * *"Imagine the code you are writing, whatever it is for, is an NPM/Nuget package."*.
  * This mindset promotes creating reusable code with room for reinterpretation.
* **TDD**: Theoretically great in pre-defined toy scenarios, practically not that important. Create tests, but it's not necessary to religiously and rigorously create all tests before all of your functional code.
* **Thoughts on SOLID**:
  * General observations:
    * Agree with the "spirit" of it.
    * It's based on somewhat imperative OOP concepts from 90's/00's era of CS academia.
    * Involves toy scenarios like "Animal, Cat, Dog", "Book, Invoice", etc.
    * Generally too absolutist. Too "0 or 1".
    * Therefore requires naunced, practical interpretation and application for real-world relevance.
  * SR principle
    * The phrase quoted often here is "There should never be more than one reason for a class to change."
    * Originates from https://web.archive.org/web/20150202200348/http://www.objectmentor.com/resources/articles/srp.pdf
    * In my experience, it's almost never optimal to separate your modules so much such that they do exactly *one* thing and only ever have <=1 reasons to change.
    * I personally believe in a more forgiving version - RM principle - Responsibility Minimization principle
      * For example: *"The purpose of your modules should be as close to one as possible and elevator-pitchable"*
  * OC principle
    * "**O**pen to extension, **C**losed to modification."
    * Relates to being able to use a class from a library and be able to extend from it without modifying the library
    * It's definition is rather verbose and meandering. Comes from 1988.
    * The closest principle of mine I have to this is "LDD" (see above *LDD* section).
  * LS principle
    * "**L**iskov-**S**ubstitution principle"
    * It's formal definition is highly academic and rather verbose, meandering, and antiquated. Comes from 1994.
    * Agree with sentiment, but prefer a practical phrasing. For example: *"Don't write hidden logic/magic that differentiates your concretions to referers."*
  * IS principle
    * Sounds nice in CS academic context, impossible in practice.
    * It's never possible in any decently-sized repository of code to tailor every module/service/thing for every other module/service/thing via interfaces that take subsets of properties. End up with too many interfaces => cognitive complexity.
    * I prefer a practical interpretation: *"Avoid giving things access to unnecessary information"*.
  * DI principle
    * Strongly agree.
    * Break down a problem and solve it with layered architectures.
    * Build your services pyramid.
    * *"Create modules that depend on libraries that depend on modules that depend on libraries that depend on...etc."*
* Why tech can fail:
  * Non-technical leaders
    * More likely to lack quality gauge
    * More likely for decisions to be deferred, leading to "death by commitee".
    * Examples: Boeing, NASA (Challenger), etc.
  * Acceptance of deviance
    * Refered to in many ways: *"Slippery slope"*, *"Death by a thousand cuts"*, etc.
    * Sometimes practicality wins here
