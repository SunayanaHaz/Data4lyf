# Where Technology Fails: An Accessibility Analysis of Real-World Websites

## Abstract
This project analyzes real-world web accessibility violations to identify systemic patterns of exclusion in digital systems. Using the AccessGuru dataset, we examine where accessibility failures occur most frequently, which violation types dominate, and which pages cause the greatest harm to users.

---

## Dataset
- 3,524 accessibility violations
- ~591 unique web pages
- Domains: News & Media, Government, Health, Education, Technology, E-commerce

---

## Data Preparation
- Standardized domain category labels
- Removed unsuccessfully scraped pages
- Aggregated violations at page and domain levels
- Verified consistency between severity scores and impact labels

---

## Key Findings

### 1. Accessibility Failures Are Unevenly Distributed
News & Media websites exhibit the highest concentration of accessibility violations, followed by Government and Technology domains.

![Violations by Domain](violations_by_domain.png)

---

### 2. A Small Set of Violations Dominate
Color contrast issues, missing landmarks, unclear link names, and structural HTML errors account for most accessibility failures.

![Top Violations](top_violation_types.png)

---

### 3. Severity Matters More Than Volume
We introduce a severity-weighted Risk Score to identify pages that cause the greatest harm to users.

---

## Risk Score Methodology

Risk Score is calculated as:

- 5 × Critical
- 4 × Serious
- 3 × Moderate
- 2 × Minor

This prioritizes user harm over raw violation counts.

![Risk Score Ranking](risk_score_pages.png)

---

## Human Impact
Accessibility failures disproportionately affect:
- Screen reader users
- Users with low vision
- Users relying on keyboard navigation

These issues create invisible but significant barriers to access.

---

## Recommendations
- Enforce WCAG color contrast standards
- Use semantic HTML landmarks
- Ensure descriptive link text
- Validate page structure and unique IDs

---

## Conclusion
Accessibility violations are systemic, measurable, and fixable. Data-driven analysis can guide organizations toward more inclusive digital systems.

---

## Reproducibility
All analysis was conducted using Python. Code and outputs are available in the accompanying repository.
