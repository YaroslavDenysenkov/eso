---
date: <% tp.file.title.split(" ")[0] %>
---
<%*
const date = tp.date.now("YY-MM-DD");
const folder = tp.file.folder(true);

async function createNote(templateName, fileName) {
  const existing = app.vault.getAbstractFileByPath(`${folder}/${fileName}.md`);
  if (!existing) {
    const template = tp.file.find_tfile(templateName);
    await tp.file.create_new(template, fileName, false, folder);
  }
}

await createNote("Daily Fit Template",   `${date} Daily Fit`);
await createNote("Daily Learn Template", `${date} Daily Learn`);
await createNote("Daily Me Template",    `${date} Daily Me`);
await createNote("Daily Tasks Template",    `${date} Daily Tasks`);
%>
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Fit|Daily Fit]]
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Learn|Daily Learn]]
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Me|Daily Me]]
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Tasks|Daily Tasks]]

- [ ] Daily Fit  📅 <% tp.file.title.split(" ")[0] %>

---
![[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Fit|Daily Fit]]

---

![[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Learn|Daily Learn]]

---
![[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Me|Daily Me]]

---
![[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Tasks|Daily Tasks]]
