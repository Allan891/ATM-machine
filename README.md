ATM Machine in Prolog (DD1351 - Logic for Computer Scientists)

Model Checking for CTL
The main puspose of this project is to explore model-checking techniques for Computational Tree Logic (CTL) and implement a proof system tailored for CTL formulas. Model checking is used to verify CTL formulas and is implemented here recursively, while addressing challenges posed by loops in the model, which are critical for ensuring termination.

The development process consisted of three main steps:
1. Understanding the system.
2. Implementing the system.
3. Validating its functionality through different scenarios.

Initially, the simplest possible case was tested by implementing literal evaluations, checking whether a given start node possessed a specific property.
In the second step, each successor rule was implemented and tested individually in different scenarios by writing simple models and assertions.
The final step in model checking development involved testing more complex nested rules and running the accompanying test cases. A copy of the model checker was created to log each rule that the model deemed true when evaluating a given assertion. This debugging method was useful for isolating errors whenever the program produced incorrect results or became unresponsive. The solution was then refined by testing it against various similar scenarios.

Model
The model consists of 12 states, representing a simplified version of an ATM machine. The states and properties are named in a way that makes them self-explanatory.
The model illustrates the various states required to access an account, allowing users to either view their balance or withdraw money. It also accounts for cases where a withdrawal is denied and includes branches that handle scenarios involving incorrect PIN entries, showing the possible state transitions in such cases.

The file ATM-machine.prolog is included the for this project.
