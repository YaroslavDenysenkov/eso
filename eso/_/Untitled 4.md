
```tracker
folder: 10 Journal/10 Daily
startDate: 2025-12-01
endDate: 2025-12-31
dateFormat: YYYY-MM-DD
dataset:
  - searchType: text
    searchTarget: "vocab_total"
    color: green
    name: Actual
  - color: yellow
    name: Goal
    expression: (moment(date).diff(moment("2025-12-01"), 'days') + 1) * 20
line:
    title: "Vocabulary Progress"
    yMin: 0
    yMax: 600
    showLegend: true
    fillGap: true