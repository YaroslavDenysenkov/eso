```tracker
searchType: frontmatter
searchTarget: vocab_total
folder: 10 Journal/10 Daily
startDate: 2025-12-01
endDate: 2025-12-31
dataset: 
  - color: green
  - color: yellow
    expression: (moment(date).diff(moment("2025-12-01"), 'days') + 1) * 20
line:
    title: "Vocabulary Progress (Target: 600)"
    yAxisLabel: Total Words
    lineColor: "#4caf50"
    yMin: 0      
    yMax: 600    
    yAxisTickInterval: 100
    showPoint: true
    showLine: true
    fillGap: true
    