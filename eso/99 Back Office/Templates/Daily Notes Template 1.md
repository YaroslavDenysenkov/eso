 <% tp.date.now("YYYY-MM-DD") %> Periodic Note

## Links
- [[<% tp.date.now("YYYY-MM-DD") %> Fitness]]
- [[<% tp.date.now("YYYY-MM-DD") %> Learning]]
- [[<% tp.date.now("YYYY-MM-DD") %> State]]

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

// create Learning note
await tp.file.create_new(
  tp.file.find_tfile("Daily Lern Template"),
  `${date} Learning`,
  false,
  "Periodic"
)

// create State note
await tp.file.create_new(
  tp.file.find_tfile("Daily Me Template"),
  `${date} State`,
  false,
  "Periodic"
)
%>
