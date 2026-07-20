# scemas
# BigBasket PageSpeed Scoring Workbook

## Overview

The **BigBasket PageSpeed Scoring Workbook** is an automated Excel-based website performance evaluation tool designed to measure and calculate PageSpeed scores using weighted scoring formulas.

The workbook evaluates the website based on four major Google Lighthouse categories:

- **Performance**
- **Accessibility**
- **Best Practices**
- **SEO**

Each category contains multiple sub-factors with predefined weights. The workbook automatically calculates category scores, overall website score, and quality status.

# Workbook Structure

## Level 1 - Website Score (Category Roll-Up)

This section provides the final website evaluation.

| Category       | Description                             |
| -------------- | --------------------------------------- |
| Performance    | Website speed and loading metrics       |
| Accessibility  | Website usability for all users         |
| Best Practices | Security and development best practices |
| SEO            | Search Engine Optimization metrics      |
| Overall Score  | Weighted average of all categories      |

## Level 2 - Sub-Factor Breakdown

Each category is divided into individual scoring metrics.

Example:

### Performance

- First Contentful Paint
- Largest Contentful Paint
- Speed Index
- Total Blocking Time
- Cumulative Layout Shift

### Accessibility

- Color Contrast
- ARIA Labels
- Keyboard Navigation
- Screen Reader Support
- Form Labels
- Image Alt Text

### Best Practices

- HTTPS
- Browser Errors
- Image Optimization
- Security Headers
- Deprecated APIs
- JavaScript Quality

### SEO

- Meta Title
- Meta Description
- Structured Data
- Crawlability
- Mobile Friendliness
- Canonical URL

# Scoring Method

Every metric has:

- A Weight
- A Score (0-100)

The workbook calculates the weighted score using Excel formulas.

Example:

Category Score = SUMPRODUCT(Score Range, Weight Range)

The overall website score is calculated using:

Overall Score = SUMPRODUCT(Category Weight, Category Score)

# Status Scale

| Score    | Status            |
| -------- | ----------------- |
| 90-100   | Excellent         |
| 80-89    | Good              |
| 70-79    | Average           |
| 50-69    | Needs Improvement |
| Below 50 | Poor              |

# Formula Automation

The workbook is designed to minimize manual calculations.

Automated calculations include:

- Category Score
- Weighted Score
- Overall Website Score
- Final Status

Users only need to enter metric scores (where applicable); all totals and summaries update automatically.

# Weight Distribution

| Category       | Weight |
| -------------- | ------ |
| Performance    | 25%    |
| Accessibility  | 25%    |
| Best Practices | 25%    |
| SEO            | 25%    |

Total Weight = **100%**

# How to Use

- Open the workbook in Microsoft Excel.
- Navigate to the **Level 2** section.
- Enter or update individual metric scores (0-100) if they are not already formula-driven.
- Verify that each metric has the appropriate weight.
- Review the automatically calculated category scores.
- Check the **Overall Website Score** displayed in the Level 1 summary.
- Use the status column to assess website quality.

# Features

- Fully automated score calculation
- Weighted scoring model
- Category-wise performance analysis
- Overall website health score
- Easy to customize
- Professional reporting format
- Excel formula-driven calculations
- Scalable for additional metrics

# Formula References

The workbook uses Excel functions such as:

- SUMPRODUCT()
- SUM()
- AVERAGE()
- IF()
- ROUND()

These formulas automatically update all dependent calculations whenever input values change.

# Recommended Workflow

- Run Google Lighthouse or PageSpeed Insights for the website.
- Record the individual metric scores.
- Update the workbook.
- Review category scores.
- Identify low-scoring areas.
- Implement performance improvements.
- Re-run Lighthouse and compare results.

# Requirements

- Microsoft Excel 2019 or later (Microsoft 365 recommended)
- Formula calculations enabled
- Macros are **not required**

# Notes

- Do not overwrite formula cells.
- Modify only input cells intended for score entry.
- Adjust weights if your evaluation methodology changes.
- Keep a backup before making structural modifications.

# Version

**Workbook Version:** 1.0

**Purpose:** Website Performance & Lighthouse Scoring

**Platform:** Microsoft Excel

**Maintained By:** Your Organization / Team
