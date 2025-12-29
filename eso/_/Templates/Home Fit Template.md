<%* const fileName = "Home Fit " + tp.date.now("YYYY-MM-DD [W]ww ddd"); await tp.file.rename(fileName); %>

---
date: <% tp.file.creation_date("YYYY-MM-DD") %>
tags: [workout]
fit_pt_pushup:
fit_pt_captain:
fit_pt_dip_tricep:
fit_pt_dip_chest:
---

# Workout: <% tp.date.now("YYYY-MM-DD") %>


| Power Tower |                                   |
| ----------- |:--------------------------------- |
| Push Ups    | `INPUT[number:fit_pt_pushup]`     |
| Captain     | `INPUT[number:fit_pt_captain]`    |
| Tricep Dips | `INPUT[number:fit_pt_dip_tricep]` |
| Chest Dips  | `INPUT[number:fit_pt_dip_chest]`  |


