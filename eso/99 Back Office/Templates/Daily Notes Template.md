
## Links

- [[<% tp.file.folder() %>/<% tp.date.now("YY-MM-DD") %> [Daily Fit]|Daily Fit]]
- [[<% tp.file.folder() %>/<% tp.date.now("YY-MM-DD") %> [Daily Learn]|Daily Learn]]
- [[<% tp.file.folder() %>/<% tp.date.now("YY-MM-DD") %> [Daily Me]|Daily Me]]


## Links
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> [Daily Fit]]]
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> [Daily Learn]]]
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> [Daily Me]]]


- [[<% tp.file.folder() %>/<% tp.date.now("YY-MM-DD") %> [Daily Fit]]]
- [[<% tp.file.folder() %>/<% tp.date.now("YY-MM-DD") %> [Daily Learn]]]
- [[<% tp.file.folder() %>/<% tp.date.now("YY-MM-DD") %> [Daily Me]]]


- [[<% tp.file.folder() %>/<% tp.date.now("YYYY-MM-DD") %> Daily Fit]]
- [[<% tp.file.folder() %>/<% tp.date.now("YYYY-MM-DD") %> Daily Learn]]
- [[<% tp.file.folder() %>/<% tp.date.now("YYYY-MM-DD") %> Daily Me]]

- [[<% tp.date.now("YYYY-MM-DD") %> Daily Fit]]
- [[<% tp.date.now("YYYY-MM-DD") %> Daily Learn]]
- [[<% tp.date.now("YYYY-MM-DD") %> Daily Me]]

<%*
const date = tp.date.now("YY-MM-DD");
const folder = tp.file.folder(true);

async function createIfMissing(templateName, fileName) 
{
 
 const existing = app.vault.getAbstractFileByPath(`${folder}/${fileName}.md`);

  if (!existing) 
  {
    const template = tp.file.find_tfile(templateName);
    await tp.file.create_new(template, fileName, false, folder);
  }
}

await createIfMissing("Daily Fit Template",   `${date} Daily Fit`);
await createIfMissing("Daily Learn Template", `${date} Daily Learn`);
await createIfMissing("Daily Me Template",    `${date} Daily Me`);
%>
