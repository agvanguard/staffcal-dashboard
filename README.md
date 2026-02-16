# StaffCal Dashboard

CHT Staffing Calendar Dashboard - A workforce management tool for visualizing staffing schedules, forecasts, and net staffing levels.

## Features

- 📊 **CSV Import/Export** - Load data from Google Sheets
- 📅 **Interactive Calendar** - Monthly view with staffing metrics
- 🔍 **Advanced Filtering** - Filter by Queue (LOB) and Channel
- ⏰ **Hourly Breakdown** - 24-hour staffing analysis
- 🎨 **Color-Coded Display** - Visual staffing level indicators
- 📈 **Aggregated Views** - Sum across all queues or channels

## Quick Start

1. Download the CSV from Google Sheets
2. Open `staffcal.html` in your browser
3. Click "Import Files" and select your CSV
4. Use filters to analyze specific teams
5. Click any date for detailed hourly breakdown

## CSV Format (Columns A-H)

- **Column A**: Date
- **Column B**: Time (for hourly breakdown)
- **Column C**: Start Time (not used)
- **Column D**: Channel (email, chat, etc.)
- **Column E**: Queue (department/LOB name)
- **Column F**: Staffing Scheduled
- **Column G**: Staffing Required - Forecasted
- **Column H**: Staffing Net

## Calculations

- **Daily Scheduled** = Sum of Column F ÷ 7.5
- **Daily Required** = Sum of Column G ÷ 7.5
- **Daily Net Staffing** = Scheduled - Required
- **Hourly Values** = Sum of Column H per hour interval

## Technologies

- Pure HTML/CSS/JavaScript
- No dependencies required
- Works offline after download

## License

MIT License
```

---

## 🎯 **Quick GitHub Desktop Method (No Command Line)**

1. Download [GitHub Desktop](https://desktop.github.com)
2. Open GitHub Desktop → **"Create New Repository"**
3. Name it `staffcal-dashboard`
4. Choose a local path
5. Click **"Create Repository"**
6. Copy your `staffcal.html` file into that folder
7. GitHub Desktop will show the file
8. Add commit message: "Initial commit"
9. Click **"Commit to main"**
10. Click **"Publish repository"** to push to GitHub

---

## 📦 **Recommended Repository Structure**
```
staffcal-dashboard/
├── README.md
├── staffcal.html
├── .gitignore (optional)
└── docs/
    ├── screenshots/
    └── user-guide.md
