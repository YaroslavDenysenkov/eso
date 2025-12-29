
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
