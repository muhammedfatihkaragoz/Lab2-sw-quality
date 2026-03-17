# SENG272 Lab 2 - ISO/IEC 25010 Software Quality Evaluation

This project evaluates software system quality using ISO/IEC 25010 quality characteristics and ISO/IEC 25023 measurement metrics. The system is implemented using Java OOP principles and Collections Framework (ArrayList, HashMap).

## Features
- Criterion-based scoring system
- Quality dimension evaluation (ISO/IEC 25010)
- Overall system quality score calculation
- Weakest dimension detection (gap analysis)
- Console-based formatted report

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

## ISO/IEC 25023 Metric Reference

| Characteristic | Metric | Direction | Unit |
|---------------|--------|----------|------|
| Functional Suitability | Functional Completeness Ratio | Higher | % |
| Functional Suitability | Functional Correctness Ratio | Higher | % |
| Reliability | Availability Ratio | Higher | % |
| Reliability | Defect Density | Lower | defect/KLOC |
| Performance Efficiency | Response Time | Lower | ms |
| Performance Efficiency | CPU Utilisation | Lower | % |
| Maintainability | Test Coverage Ratio | Higher | % |
| Maintainability | Cyclomatic Complexity | Lower | score |

## Notes
- Scores are normalized between 1 and 5
- Results are rounded to nearest 0.5
- Weighted averages are used for dimension scores
- Overall score is calculated based on dimension weights
