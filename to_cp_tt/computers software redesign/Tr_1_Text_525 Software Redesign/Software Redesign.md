
[Dummied Out - TV Tropes](https://tvtropes.org/pmwiki/pmwiki.php/Main/DummiedOut)
- older hardware (i.e., when coded straight to firmware) requires invalidating code more than removing it
    - it opens up opportunities for [hacking] as well!

freeCodeCamp dev quiz - Software Redesign

- An IndexError is raised in Python when you try to index a list, tuple, or string beyond the permitted boundaries.
- A RecursionError in Python occurs when the interpreter detects that the maximum recursion depth is exceeded. This usually occurs when the recursive process never reaches the base case.
- A NameError is raised in Python when a name that you are referencing in the code doesn't exist.
- A ZeroDivisionError is raised in Python when you try to divide by zero.
- A KeyError is raised in Python when you try to access the value of a key that doesn't exist in a dictionary.
- A TypeError is raised in Python when an operation or function is applied to an object of an inappropriate type.
- Function overloading is when you have multiple functions with the same name but with different parameters. This results in the function being overloaded with different jobs.
- Hoisting is the process of moving variables, classes, and functions to the top of the scope.

Here's a couple considerations that factor into being a good QA engineer:

- Do you take the time to understand why the bug is happening?
    Alongside the clearly defined and reproducible steps, do you have
    insight into why the issue might be occurring and how to fix it? Is
    there a similar bug from the past that might help? Can you point to the
    exact lines of code responsible for this bug? (You might think this last one is crazy but I've had QA engineers that did this and I was beyond
    impressed)
- Do you take the time to make complicated or not easily reproducible bugs more reproducible?
- If there are tests that the devs need to run themselves, have you automated or streamlined that process?
- Have you grokked the code base and understood how the app
    functions? This is important because it allows you to have a better
    understanding of what is a trivial bug and what is a significant
    undertaking, allowing your team better planning.
- Do you stay actively involved throughout the sprint and know when requirements have changed? Instead of making it the responsibility of
    the devs to include you, do you include yourself since you know it's
    relevant to your testing?
- Do you anticipate bugs that may arise with new features and preemptively point them out as requirements?
