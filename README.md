# Workout Template Generator

A single-file web app that generates Excel (.xlsx) workout tracking spreadsheets. No installation required — runs entirely in your browser.

**[Use it now](https://dangervalentine.github.io/workout-template-generator/)**

## What it does

- Pick a preset program or build your own from scratch
- Optionally set starting weight, reps, and sets per exercise
- Download a formatted .xlsx spreadsheet that tracks your progress week by week

## How the spreadsheet works

Each exercise gets four columns per week:

| Column | Purpose |
|--------|---------|
| **Weight** | The weight you plan to lift |
| **Reps** | Target reps per set |
| **Sets** | Number of sets |
| **Amount** | Reps you actually hit on your last set |

Week 1's values carry forward automatically — each subsequent week copies the previous week's Weight/Reps/Sets until you manually change them in the spreadsheet. The **Amount** column color-codes each week based on how you performed relative to your target, helping you decide when to adjust.

Adjusting your plan is a manual decision. The spreadsheet gives you the data; you make the call on when to progress or dial back.

## Included templates

- Basic Upper/Lower
- StrongLifts 5x5
- Madcow 5x5
- Texas Method
- Upper/Lower Split
- Push/Pull/Legs

## Technical details

- Single HTML file (~970 KB) with [ExcelJS](https://github.com/exceljs/exceljs) embedded inline
- Works fully offline after first load
- No server, no build step, no dependencies to install
- Cross-platform: Windows, macOS, Linux — anything with a browser
