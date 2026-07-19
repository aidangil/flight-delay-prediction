# Flight Delay Risk Analysis Using Monte Carlo Simulation (Excel)

## Project Overview

This project uses **Monte Carlo simulation in Microsoft Excel** to evaluate the risk of missing a connecting flight when flying with Spirit Airlines. By simulating **10,000 possible flight scenarios** under different airport arrival times, the model estimates the probability of missing a flight while accounting for uncertainty in flight delays, TSA security wait times, and walking time to the departure gate.

The analysis helps travelers balance the tradeoff between arriving early enough to avoid missing a flight while minimizing unnecessary waiting at the gate.

---

## Business Problem

Air travelers frequently struggle with determining **how early they should arrive at the airport**. Arriving too early results in unnecessary waiting, while arriving too late increases the risk of missing a flight.

This project answers the question:

> **How does arrival time before departure affect average waiting time and the probability of missing a flight?**

---

## Data

The simulation was built using historical information representative of **Spirit Airlines operations** and incorporates several uncertain variables:

- Flight delay distributions
- TSA security screening times
- Walking distance/time to the departure gate
- Scheduled airport arrival times

Three arrival scenarios were analyzed:

- **30 minutes before departure**
- **45 minutes before departure**
- **60 minutes before departure**

Each scenario was simulated using **10,000 Monte Carlo iterations**.

---

## Analysis Performed

The Excel model generates thousands of randomized flight scenarios by sampling from probability distributions for each uncertain variable.

For every simulation, the model calculates:

- Flight delay
- TSA security wait time
- Walking time to the gate
- Total time required to reach the gate
- Remaining wait time before boarding
- Whether the passenger misses the flight

The simulation results are then aggregated to estimate:

- Average waiting time
- Average security screening time
- Average flight delay
- Probability of missing the flight

---

## Key Findings

### 30-Minute Arrival

- **Average gate wait:** ~8.9 minutes
- **Probability of missing flight:** ~42.7%

Arriving only 30 minutes before departure provides very little buffer against variability in airport operations, resulting in a high likelihood of missing the flight.

---

### 45-Minute Arrival

- **Average gate wait:** ~20.9 minutes
- Significantly lower risk of missing the flight while maintaining a reasonable waiting time.

This arrival window represents a more balanced tradeoff between convenience and reliability.

---

### 60-Minute Arrival

- **Average gate wait:** ~35.3 minutes
- Lowest risk of missing the flight, but with considerably longer idle time before boarding.

This option prioritizes reliability over minimizing wait time.

---
