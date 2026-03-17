# SENG272 Lab 2 - ISO/IEC 25010 Software Quality Evaluation

This project implements a software quality evaluation system based on ISO/IEC 25010 and ISO/IEC 25023.

## Features
- Criterion-based scoring system
- Quality dimension evaluation
- Overall system quality score
- Weakest dimension analysis

## Project Structure
- src/
  - Criterion.java
  - QualityDimension.java
  - SWSystem.java
  - SWSystemData.java
  - Main.java

## ISO Reference
This project uses ISO/IEC 25010 and ISO/IEC 25023 quality metrics for evaluation.

## ISO/IEC 25010 Quality Characteristics

| Dimension | Code | Metrics |
|----------|------|--------|
| Functional Suitability | QC.FS | Functional Completeness, Functional Correctness |
| Reliability | QC.RE | Availability, Defect Density |
| Performance Efficiency | QC.PE | Response Time, CPU Utilisation |
| Maintainability | QC.MA | Test Coverage, Cyclomatic Complexity |
