# Surgical Equipment Supplier Selection using AHP-TOPSIS

## Project Overview

This repository contains a comprehensive implementation of a Multi-Criteria Decision-Making (MCDM) framework for selecting the optimal 
suppliers of surgical equipment for healthcare institutions. 
The project addresses the complex challenge of evaluating suppliers based on multiple competing criteria, 
including cost, quality, delivery time, reliability, and regulatory compliance.

## Business Problem

Healthcare institutions face significant challenges when selecting suppliers for critical surgical equipment:

- Poor supplier choices can compromise patient safety
- Multiple criteria must be balanced simultaneously (cost vs. quality vs. reliability)
- Decision makers need a systematic, data-driven approach rather than subjective judgments
- Healthcare regulations require detailed justification for procurement decisions

This project provides a structured methodology that transforms a complex decision problem into a systematic, 
quantifiable process using established MCDM techniques.

## Methodology

The implementation combines two powerful decision-making methods:

### 1. Analytic Hierarchy Process (AHP)
- Establishes the relative importance of each decision criterion
- Creates a pairwise comparison matrix based on expert judgment
- Calculates normalized eigenvectors to determine criteria weights
- Performs consistency checks to validate the weight assignments

### 2. Technique for Order Preference by Similarity to Ideal Solution (TOPSIS)
- Normalizes the decision matrix to make criteria comparable
- Applies weights from AHP to the normalized matrix
- Identifies ideal and negative-ideal solutions for each criterion
- Calculates separation measures and relative closeness to the ideal solution
- Ranks suppliers based on their performance across all criteria

## Features

- **Comprehensive Data Analysis**: Handles real-world supplier data with multiple criteria
- **Customizable Weighting**: Allows adjustment of criteria importance based on institutional priorities
- **Product Category Analysis**: Identifies top suppliers for specific surgical equipment types
- **Visualization**: Includes intuitive charts and graphs for decision support
- **Sensitivity Analysis**: Tests the robustness of rankings against variations in criteria weights
- **Consistency Validation**: Ensures logical consistency in subjective weight assignments

## Dataset

The dataset contains information about 100 suppliers of surgical equipment including:
- Supplier identification
- Product categories (scalpels, forceps, surgical scissors, retractors, needle holders)
- Cost per unit (INR)
- Quality ratings (1-10)
- Delivery time (days)
- Reliability scores (1-10)
- Flexibility in handling orders (1-10)
- Regulatory compliance (1-10)
- Sterility standards (1-10)
- After-sales support quality (1-10)

## Implementation

The project is implemented in Python, utilizing libraries including:
- NumPy and Pandas for data manipulation
- SciPy for mathematical operations
- Matplotlib and Seaborn for visualization

## Usage

The implementation follows a modular structure that allows users to:
1. Load and preprocess supplier data
2. Define criteria importance through pairwise comparisons
3. Generate AHP weights with consistency checking
4. Apply TOPSIS for ranking alternatives
5. Analyze results by product category
6. Visualize rankings and criteria performance
7. Perform sensitivity analysis

## Results

The output includes:
- A ranked list of suppliers based on their overall performance
- Category-specific rankings for different surgical equipment types
- Visual comparisons of top suppliers across evaluation criteria
- Sensitivity analysis showing the stability of rankings to weight changes

## Future Enhancements

Potential extensions to this project include:
- Integration with procurement systems
- Web-based interface for interactive decision support
- Inclusion of additional MCDM methods (ELECTRE, PROMETHEE)
- Dynamic weight adjustment based on changing healthcare priorities
- Machine learning integration for predictive supplier performance

