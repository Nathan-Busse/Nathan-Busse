![](Thimbnail_with_background_small.png)

Imagine you have an old, messy house full of outdated wiring and appliances that nobody wants to touch because fixing one thing might break another. **Exodus** is like a team of seven tiny, tireless electricians who move into that house, study every wire, figure out what needs to change, make the changes, test every light switch, fix anything they broke, and even go to the hardware store to buy missing parts – all while you’re away. When they’re done, the house is modern, safe, and everything works, and they’ve left a neat note explaining what they did.

More concretely, Exodus is a **self‑driving code migrator**. You give it an old Python script (or an entire project) and tell it, “I want to switch from `stripe` to `stripe_v2`” (or any other library). Exodus then:

1. **Maps** your code to understand every import and dependency.  
2. **Strategizes** what needs to change.  
3. **Rewrites** the code surgically, without touching anything else.  
4. **Runs your tests** in a safe, isolated container to see if the changes work.  
5. If tests fail, it **autopsies** the error, figures out whether the migration itself was a bad idea or if a required package is missing, and either reverts the change or installs the missing package.  
6. It repeats this loop until **all tests pass**.  
7. Finally, it **remembers** what worked (and what didn’t) so future migrations are even faster.

You can use Exodus from a terminal or a sleek, accessible GUI. It works on single files, whole folders, and even projects that don’t have any tests yet – it will create a simple test for you just to make sure everything imports correctly. The whole process is hands‑off: you provide the target, and Exodus delivers a working, modernized codebase.
