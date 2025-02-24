ATM Machine in Prolog (DD1351 - Logic for Computer Scientists)

Model Checking for CTL

The main purpose of this assignment is exploring (model checking) techniques for computational tree logic (CTL), and implementing a proof system tailored for CTL formulas. Model checking is used for verification of CTL formulas and is here implemented recursively while addressing the challenges posed by loops within the model, which is critical for ensuring termination.

The approach to this assignment has three steps: 

1. Understanding the system.

2. Implementing the system.

3. Validating its functionality through different scenarios. 


I started out by making a skeleton version of the program that could handle the easiest possible case by implementing the literals and checking whether a given start node had a specific property or not.

Step two was implementing every subsequent rule and testing them separately in different scenarios by writing simple models and statements. 

The final step of the model checker development was testing with more complicated statements nesting multiple rules and running through the provided test suite. We made a copy of our model checker that would write out every rule the model judged as being true while testing a statement and used it if the program gave a incorrect answer or froze on a test file to isolate the problem. Then we ran the updated solution through various similar scenarios.


Model

The model consists of 12 states and represents a simplified version of a ATM-machine. The states and properties are named in a way that makes them pretty self-explanatory. In short the model shows the different states in accessing a account and either displaying the account balance or withdrawing money. It does also account for the possibility of the withdrawal being denied as well as having a branch for showing the different states and possible transitions in the eventuality of a incorrect pin being entered.

The file ATM-machine.prolog include the code for this project.
