This project explores name-based hiring discrimination by analyzing how perceived ethnicity (inferred from “Caucasian-sounding” vs. “African American–sounding” names) affects the likelihood of receiving a callback from employers. The dataset originates from a landmark field experiment conducted by Bertrand and Mullainathan (2004), which involved sending 4,870 fictitious resumes with randomly assigned names to real job postings in Chicago and Boston. By holding resume qualifications constant and varying only the names, the experiment isolates whether employers respond differently based on perceived ethnicity.

Key Steps
Data Acquisition and Preparation

Source: Cross-sectional data from Bertrand and Mullainathan (2004).
Structure: 4,870 rows, each representing a single resume, including variables for experience, “quality” tier, industry, and whether or not a callback occurred.
Cleaning: Removal of incomplete entries, conversion of categorical columns (e.g., gender, ethnicity) into numeric/binary indicators, and validation of numeric fields (such as experience).
Exploratory Data Analysis (EDA)

Descriptive Statistics: Basic metrics (counts, means, distributions) to understand data balance and potential outliers.
Pivot Tables: Computed average callback rates for different industries and ethnicities, revealing a consistent higher callback rate for resumes with Caucasian-sounding names.
Visualizations: Bar plots, grouped bar charts, and histograms to highlight disparities, especially across different industries.
Logistic Regression Model

Variables: Experience, gender, perceived ethnicity, and resume quality (plus a dummy variable for college attendance).
Findings:
Experience significantly increases the odds of a callback.
Ethnicity (Caucasian) shows a strong, statistically significant positive effect on receiving a callback.
Gender and college do not exhibit statistical significance in the tested model.
The model’s pseudo R-squared is modest (~0.013–0.014), common for social-science data, but p-values confirm the robust effect of perceived ethnicity.
Industry-Specific Insights

A pivot table summarizing callback rates by industry suggests that finance/insurance/real estate and business/personal services display larger ethnic disparities, whereas manufacturing and trade show smaller (but still present) gaps.
Conclusions and Implications
Perceived ethnicity (signaled by names) remains a strong predictor of callback likelihood, implying systemic bias.
Even after controlling for experience and resume quality, resumes with Caucasian-sounding names consistently received more callbacks across multiple industries.
Results highlight ongoing challenges in achieving equitable hiring practices, indicating the need for interventions such as blind review, structured interviews, or broader bias-awareness initiatives.
Future Directions
Refined Models: Multi-level or hierarchical modeling could capture employer- or industry-specific variances more effectively.
Additional Features: Incorporating other resume aspects (e.g., volunteer work, honors, military experience) could reveal how additional credentials interact with name-based perceptions.
Broader Datasets: Validating these findings with modern online application platforms or across different geographic locations would help assess whether name-based hiring discrimination persists at scale.
