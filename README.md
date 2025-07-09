# SA2025finalprojectbyzeba
final ML project of summer analytics 2025 program of IIT gwahati's c&amp;a club

 # Dynamic Pricing System for Urban Parking Lots

This project addresses the challenge of dynamic pricing in urban parking zones by using real-time and historical factors to compute optimal prices. The solution was developed as part of **Summer Analytics 2025** by the Consulting & Analytics Club, IIT Guwahati.

==================


# Overview

Urban cities often face parking congestion, stockouts, and underutilization due to static pricing. This project creates a three-layered pricing system for parking lots:

- **Model 1**: Baseline (fixed rate)
- **Model 2**: Demand-based pricing (based on queue length, occupancy, weather, vehicle type, etc.)
- **Model 3**: Competitive pricing (adjusts price based on nearby lots and demand)
- Also integrated **real-time streaming** simulation using **Pathway**, making the solution dynamic and deployable.

====================

# Tech-Stack used 


## 🛠 Tech Stack

- **Python 3.10+**
- **Pandas** & **NumPy** — data manipulation
- **Pathway** — real-time data streaming and transformation
- **Bokeh** — interactive price visualizations
- **Google colab** — development environment

=======================

# Architecture Diagram (Mermaid)

```mermaid
graph TD
  A[Dataset: Parking Lot Info] --> B[Preprocessing & Feature Engineering]
  B --> C[Model 1: Fixed Pricing]
  B --> D[Model 2: Demand-Based Pricing]
  B --> E[Model 3: Competitive Pricing]
  E --> F[Real-time Streaming via Pathway]
  F --> G[Output: Dynamic Prices (JSONL)]
  G --> H[Bokeh Visualizer]

====================
