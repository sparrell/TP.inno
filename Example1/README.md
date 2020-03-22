# Recreating History
This example recreates history
as if this process existed previously.

## Step 1 - Convert from MS Word to Markdown
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

In this example, the files are in this directory.
For moving forward, tp_inno.md should be in main directory so it is copied to there.

Committing to repo and viewing on repo
shows conversion is not perfect.
For example, all the TD header info is present
and the figures are missing.
The figure was added, and some of the cleanup was done.
Making it 'pretty' can be done in future.

### Step 2 - Tag a Release on SG Agreement
Agreed text should be tagged with a release.

To tag tp_inno on the master branch in the main directory,
"releases" was clicked on the github repo page for TP.inno.
The form was filled out with:
- "v0.0.1"  for version numbering
- "2019.08-SG17-Agreement" for title
- "SG17 agreed to TD2484 as the currently agreed text for TP.inno" for description.

This makes it easy to get back to this version since it will always appear  on "Releases" tab of the repo.


## Step 3 - Create Issue
Changes should be proposed to address issues.
In this case it is a contrived issue to recreate C.823.
Probably multiple issues should have been created
but since this is a contrived example recreating history,
only one contrived issue will be created.

On the github repo, the issues tab was clicked
and then 'new issue' was clicked.
The form was completed with trivial text for this
contrived example.
Moving forward, real issues should be used.

## Step 4 - Create Branch to Propose changes
The master should only contain SG agreed text,
so all proposals should be made on branches.
Branches can be created on you local copy
and pushed to the repo.
Or branches can be created directly on GitHub
and fetched to you local copy.

In this case the branch "Issue-01-C823" was created.
It is good practice to have both the issue number
(albeit normally shorter eg I01) and shorthand text
on what the issue is
(normally would be more descriptive than this contrived example).

## Step  5 - Propose the Changes
Since this process didn't exist previously
(we are recreating history),
we must reconstitute the proposes changes of C.823
as markdown.
To do that, you could do it manually but for here we
will convert C.823 to markdown and diff the two markdowns.
Normally this would not have to be done.

The [C.823.docx in this directory](./XC.823.docx)
downloaded from
[T17-SG17-C-0823!!MSW-E.docx](https://www.itu.int/md/T17-SG17-C-0823/en)
on the ITU site.

It was converted to markdown using  
```
pandoc c.823.docx -f docx -t gfm -o c823.md
```
