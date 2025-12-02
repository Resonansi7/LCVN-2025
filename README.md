# LCVN-2025: Logistics Causal Vulnerability Nexus Analysis

## Causal Manifesto: The Illusion of Redundancy

This repository serves as a **Proof-of-Concept (PoC)** for the Causal Dominance framework. It is designed to prove one central thesis: **Redundancy does not guarantee stability; it only guarantees complexity.**

Traditional risk models search for failure probabilities. The **Causal Structure Learning (CSL)** approach, demonstrated here, searches for the **single point of maximum dependency**—the **Causal Nexus**—whose minimal intervention yields a catastrophic cascade.

### The Causal Debt: A Single Faulty Sensor

Our simulation targets a metropolitan cold chain logistics network. Common sense dictates that if one warehouse fails, others compensate. This PoC shows that:

1.  **A Single Obsolete Temperature Sensor (The Nexus)** reports its status to three critical, but decoupled, systems: A central inventory management system, a freight routing algorithm, and a regulatory compliance module.
2.  If this sensor is manipulated to report an **undisclosed, sub-threshold anomaly** (a gradual drift, not an outright failure), the regulatory system is forced into a mass **product recall (Actuation)** due to compliance violation, collapsing 40% of fresh supply capacity in one week.
3.  The central inventory system, designed for traditional failure modes, is too slow to react. **The system is paralyzed by a single, successful intervention.**

Prediction would have warned about "supply chain risk." **Causal Dominance** shows you the **lever** that creates the collapse.

### Repository Structure

- **1_IoT_Mapping:** Mock data for the sensor network.
- **2_CSL_Nexus_Finder:** The core Python script demonstrating CSL logic.
- **3_UmbraMaps_Viz:** Visualization of the cascade effect (Requires a simple HTML renderer).

**Your strategy is obsolete if it relies on prediction. Stop predicting the problem. Start engineering the Finality.**
