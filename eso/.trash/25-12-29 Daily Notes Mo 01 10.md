 
## Links
- [[<% tp.date.now("YYYY-MM-DD") %> Fitness]]

<%*
// store today's date
const date = tp.date.now("YYYY-MM-DD")

// create Fitness note
await tp.file.create_new(
  tp.file.find_tfile("99 Back Office/Templates/Daily Fit Template.md"),
  `${date} Fitness`,
  false,
  "Periodic"
)
%>
