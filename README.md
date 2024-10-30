# CSE259 - Project 3: Theorem Prover with Wang's Algorithm

## Team Members
- **Member 1:** Heston Hamilton
- **Member 2:** Vaughn Hoffler

Third group project for CSE 259.

## Project Overview
This project implements a theorem prover in Prolog using **Wang's Algorithm**. The prover determines the validity of logical sequents by progressively simplifying premises and conclusions through rule applications. This project provides insight into how logic programming can be leveraged to solve logical proofs programmatically.

## Project Structure

1. **Core Algorithm Implementation**
   - Uses Wang's Algorithm for logical transformations and sequent simplification.
   - Includes both **non-branching rules** (for single proof line transformations) and **branching rules** (for transformations requiring multiple proof branches).

2. **File Structure**
   - `wangs_algorithm_template.pl`: Prolog template file containing partial implementation of the algorithm with areas marked for additional rule definitions.
   - `test-cases.md`: Test cases to validate the theorem prover.

## Tasks Implemented

### Task 1: Complete Rule Definitions
- Implement the missing rule definitions in `wangs_algorithm_template.pl`:
  - **Rule 3 (Non-branching)**: For implications on the right side of the sequent, add the antecedent to the left and the consequent to the right.
  - **Rule 4 (Branching)**: For formulas with disjunction on the left or conjunction on the right, split into two separate lines, each requiring proof.

### Task 2: Validate Proof Logic
- Test each rule and ensure that transformations lead to the correct proof results.

## Running the Theorem Prover

1. Load the `wangs_algorithm_template.pl` file in your Prolog environment.
2. Run the prover by querying:
   ```prolog
   ?- prove_sequent(Premises, Conclusion).
   ```
   Replace `Premises` and `Conclusion` with the logical statements as needed.

## Testing

Use the cases in `test-cases.md` to validate that each rule performs correctly.

## Requirements

- GNU-Prolog compiler