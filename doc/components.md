
This is a list of software components for the entropy Python package.  
 
 ---
*Component name:* entropy_calculation
*Description:* Calculate the entropy of a system of states where the system is given as a list of probabilities of being in each state. The list of probabilities must sum to 1. Entropy is calculated in bits (binary), nats (natural base), and dits (decimal base), with bits being the default, if not supplied by the user. This function should only use the base `math` library and no additional imports.
*Inputs*: a list of probabilities of the available states of the system. The list must sum to 1. The list must contain positive values only. The list can as short as one item. If these rules are violated, a ValueError should be raised.
*Output*: a positive floating point value with entropy in bits, nats, or dits depending on what the user has specified.
*Side-effects:* May raise a ValueError on input validation failure.

---
