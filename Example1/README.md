# Recreating History
This example recreates history
as if this process existed previously.

In the August-2019 SG17 meeting,
TD.2484 was agreed as the current text of TP.inno.
The TD is available at [T17-SG17-190827-TD-PLEN-2484!!MSW-E.docx](https://www.itu.int/md/T17-SG17-190827-TD-PLEN-2484/en) and a copy  
[TD2484](./TD2484.docx)
is in this repo.
Note that a word doc would not normally be included
in a github repo.
It is included here as part of the example of how
to get started and also serves as the 'baseline' text.

[Pandoc](https://pandoc.org/) was used to create
the first version of tp_inno.md which was committed
(put hotlink here once committed).
The command used was:
```
pandoc td.2484.docx -f docx -t gfm -o tp_inno.md
```

- td.2484.docx was the input file
- "-f docx" means the from format is microsoft docx
- "-t gfm" means the output format is GitHub markdown
- "-o tp_inno.md" means put the output in a file called  tp_inno.md
