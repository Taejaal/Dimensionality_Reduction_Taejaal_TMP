# Dimensionality_Reduction_Taejaal_TMP

## Project Overview

This project uses **dimensionality reduction techniques** (PCA and t-SNE) to analyze high-dimensional student performance data and uncover natural groupings among students. The analysis reveals hidden patterns of performance that aren't immediately obvious from raw grade averages.

### Goal
Identify student segments based on their academic strengths and weaknesses across multiple subjects to enable targeted educational interventions and personalized learning strategies.

---

## Dataset Description

**File:** `student_grades.csv`

The dataset contains individual student grades across 8 subjects:
- **STEM Subjects:** Math, Science, Computer Science (CS)
- **Humanities:** English, History, Spanish
- **Electives:** Band, Physical Education (PhysEd)

**Structure:**
- 100 students (rows)
- 9 columns: student_id + 8 subject grades
- Grades range from 0-100

Key Findings

📊 Performance Patterns

Band has the highest average (72.1) and most consistent performance
Mathematics has the lowest average (51.6) and requires immediate intervention
Computer Science shows highest variability (std=14.1), indicating diverse skill levels
Physical Education exhibits bimodal distribution, suggesting two distinct student populations
🔗 Subject Relationships

Strong correlations within STEM subjects (r = 0.68-0.72)
Moderate correlations within Humanities (r = 0.48-0.55)
Band and Physical Education show near-zero correlation with academic subjects
📉 Dimensionality Reduction Results

PCA: First 2 components explain 55.7% of variance

PC1: Overall academic performance
PC2: STEM vs Humanities orientation
t-SNE: Revealed 6-7 distinct student subtypes invisible in PCA
UMAP: 4x faster than t-SNE with better global structure preservation
👥 Identified Student Segments

STEM-Focused High Performers (28%) - Excel in Math, Science, CS
Humanities-Focused High Performers (24%) - Excel in English, History, Spanish
Balanced Medium Performers (26%) - Average across all subjects
Low Performers (22%) - Struggle academically, especially in Mathematics
💡 Recommendations

Implement differentiated Mathematics pathways (accelerated, standard, foundational)
Develop early warning system to identify at-risk students before failure
Protect Band and Physical Education as success pathways for struggling students



## Files Included

1. **student_clustering_analysis.ipynb**
   - Complete Jupyter notebook with:
     - Data exploration and visualization
     - PCA implementation and analysis
     - t-SNE implementation with multiple perplexity values
     - Clustering and interpretation
     - Comprehensive visualizations
     - Actionable recommendations

2. **student_grades.csv**
   - Original dataset with student grades

3. **README.md** (this file)
   - Project documentation

4. **Subjective questions pdf** 

