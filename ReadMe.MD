# IIM B Term 1 CGPA Calculator

A lightweight single-page web app to calculate **Term 1 CGPA** using subject-wise scores and credit-weighted averaging.

## Overview

This project is built as a pure HTML/CSS/JavaScript calculator (no build tools, no dependencies). It lets you:

- Enter marks out of 100 for each subject.
- View grade badges instantly for each subject.
- See real-time weighted percentage and CGPA.
- Track completed credits out of total Term 1 credits.
- Handle pending subjects naturally by leaving scores blank.

## Subjects and Credits

- Marketing Fundamentals: `3`
- Financial Statements and Business Performance: `3`
- Exploration into Entrepreneurship: `1.5`
- Creativity Mindset for Innovation and Imagination (Pending): `1.5`
- Foundations of Business Communication I: `1.5`
- Evolution of Business and Market: `1.5`
- Business Statistics for Entrepreneurs I (Pending): `1.5`

Total credits: `13.5`

## Grading Scale

- `90-100`: `O`
- `80-89.99`: `A`
- `70-79.99`: `B`
- `60-69.99`: `C`
- `50-59.99`: `D`
- `< 50`: `F`

## CGPA Logic

- Weighted average is calculated as:
	- `sum(score * credits) / sum(completed_credits)`
- CGPA is displayed as:
	- `weighted_average / 10`
- The app only includes subjects with entered scores in calculation.
- If no scores are entered, values remain `0.00` CGPA and `0%`.

## Project Structure

```text
.
|- index.html
|- rEAME.MD
```

## How to Run

1. Open the project folder.
2. Open `index.html` in any modern browser.
3. Enter scores to view live CGPA updates.

No installation required.

## Customization

- Update subject list or credits in the `subjects` object inside `index.html`.
- Edit grading thresholds in the `getGrade(score)` function.
- Update social links in footer anchors:
	- `#insta-link`
	- `#linkedin-link`

## Notes

- This tool is intended for quick estimation and tracking.
- Final official CGPA should always be verified against institute records.
