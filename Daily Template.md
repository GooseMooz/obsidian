---
cssclasses: 
tags:
  - daily
---
## Yesterday undone:
[[<% tp.date.now("YYYY-MM-DD", -1) %>]]
<%* 
const today = tp.date.now("YYYY-MM-DD");
await tp.file.rename(`${today}`);
const tFileFind = tp.file.find_tfile(`${tp.date.now("YYYY-MM-DD", -1)}`);
const fileContent = await app.vault.read(tFileFind);
fileContent.split("\n").forEach(line => {
	if (line.startsWith("- [ ]")) {
		tR += `${line}\n`;
	}
})
tR = tR.slice(0, -1);
%>
## Today's plans:
- [ ] 
## Today's work:
#### New/Edited notes:

#### New ideas:

## Monthly goals progress:
