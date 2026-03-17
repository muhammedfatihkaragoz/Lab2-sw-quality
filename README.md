# SENG272 Lab 2 - ISO/IEC 25010 Software Quality Evaluation

This project evaluates software system quality based on ISO/IEC 25010 quality characteristics and ISO/IEC 25023 measurement metrics. The system is implemented using Java OOP principles and the Collections Framework (ArrayList, HashMap).

## Features
- Criterion-based scoring system using ISO/IEC 25023 metrics
- Quality dimension evaluation based on ISO/IEC 25010
- Weighted average score calculation for each dimension
- Overall system quality score calculation
- Weakest dimension identification (gap analysis)
- Console-based structured report generation

## Project Structure
- src/
  - Criterion.java
  - QualityDimension.java
  - SWSystem.java
  - SWSystemData.java
  - Main.java

## ISO/IEC 25010 Quality Characteristics

| Dimension | Code |
|----------|------|
| Functional Suitability | QC.FS |
| Reliability | QC.RE |
| Performance Efficiency | QC.PE |
| Maintainability | QC.MA |

## ISO/IEC 25023 Metric Reference (Used in this project)

This project evaluates software quality based on selected ISO/IEC 25023 metrics corresponding to ISO/IEC 25010 quality characteristics. Each metric includes its evaluation direction, measurement unit, and description.

| ISO 25010 Characteristic | ISO 25023 Metric Name | Direction | Unit | Description |
|--------------------------|----------------------|----------|------|-------------|
| Functional Suitability   | Functional Completeness Ratio | Higher | % | Indicates the proportion of implemented functions compared to planned functions |
| Functional Suitability   | Functional Correctness Ratio  | Higher | % | Measures how many functions produce correct outputs |
| Reliability              | Availability Ratio            | Higher | % | Represents system uptime relative to total operation time |
| Reliability              | Defect Density               | Lower  | defect/KLOC | Indicates number of defects per 1000 lines of code |
| Performance Efficiency   | Response Time                | Lower  | ms | Measures average response time to user requests |
| Performance Efficiency   | CPU Utilisation              | Lower  | % | Represents CPU resource usage efficiency |
| Maintainability          | Test Coverage Ratio          | Higher | % | Measures percentage of code covered by tests |
| Maintainability          | Cyclomatic Complexity        | Lower  | score | Represents code complexity and maintainability difficulty |

## Notes
- Metric scores are normalized between 1 and 5
- Scores are clamped within valid range
- Results are rounded to the nearest 0.5
- Dimension scores are calculated using weighted averages
- Overall score is calculated using dimension weights
