# PlusCal Tutorial
This repository contains code from [this](https://www.learntla.com/introduction/)
[TLA+](http://lamport.azurewebsites.net/tla/tla.html) and [PlusCal](https://www.learntla.com/pluscal/) tutorial.

TLA+ is a high-level language for modeling programs and systems -- especially concurrent and distributed ones.

PlusCal is a tool for working with TLA+: it adds a pseudocode-like interface to the specs, making them easier for programmers to understand.

## TLA+ and PlusCal Use Case
Below is an example use case where TLA+ and PlusCal and be useful.

You’re writing software for a bank. You have Alice and Bob as clients, each with a certain amount of money in their accounts. Alice wants to send money to Bob. How do you model this? Assume all you care about is their bank accounts.

One question you may have is "how can we verify that money never disappears from the system?" For example:

1. Alice wants to send $1,000 to Bob
2. System checks that Alice has enough money 
3. $1,000 is deducted from her account
4. Eve smashes the server with a baseball bat
5. Bob never receives the money
6. $1,000 has completely disappeared from the system

TLA+ and PlusCal can help you model your system in a way that it can find this bug for you.
