# OSLO Rooilijnplannen

## For editors

- first read [deze richtlijnen](https://github.com/Informatievlaanderen/OSLO-toolchain/blob/master/doc-user/README.md) .
- Use [TagsAndNotes.xlsm](https://github.com/Informatievlaanderen/OSLO-allerleiTooltjes/tree/master/EA-Excel/TagsAndNotes) 
  to edit tags in Excel. The files `*.xlsm` are included in the repo as git-ignored.


## Administrative information

### Tags
To refer to the available git tags to create a publication point from, see the "Releases" tab of this repo.


### Branches
The organisation and meaning of the git branches are documented in this table.


| Branch | Purpose | Active (y/n) |
| ------ | --------- | ---------------- | 
|  |  |  |


### Story lines

You find the story lines in the folder `story-lines`.
Each story line has a separate folder.
The title of these folders follow this template

```text
[number]-[kebab case version of title]
```

For example, the first story line with the title "Openbaar domein verbreden" has as 
folder title `1-openbaar-domein-verbreden`.

Each story line has 

- A [Markdown](https://www.markdownguide.org/basic-syntax/) file called `README.md` 
with the textual representation of the story line.
This is often an exact copy of the text that is used on the slides for the thematic working groups.
- A [JSON-LD](https://www.w3.org/TR/json-ld/) file called `data.jsonld` 
with Linked Data representation of the story line using the data model.
- An image file called `diagram.png` or `diagram.jpg` with a visual representation of the story line 
using the data model.
