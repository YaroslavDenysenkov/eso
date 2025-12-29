 
## Links
- [[<% tp.date.now("YYYY-MM-DD") %> Fitness]]

<%*
// store today's date
const date = tp.date.now("YYYY-MM-DD")

// create Fitness note
await tp.file.create_new(
  tp.file.find_tfile("Daily Fit Template"),
  `${date} Fitness`,
  false,
  "Periodic"
)
%>
