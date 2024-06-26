```toc
```
## FIXME: 
Still working on :
- Structure:
	- [x] Covert to markdown
	- [x]  Remove areas that do not make sense for unit-level training
	- [x] develop a storage structure for easy checkout
	- [x] Move to git-based solution
- Lesson Plans:
    - [ ] Classroom setup 
    - [ ] Account Authentication
    - [x] MacOS
    - [ ] Virtual Machines
    - [ ] Counter Malign Influence Terms
    - [ ] Course Start
    - [ ] Course End
    - [ ] Counter Malign Influence Capstone
    - [ ] VPN
    - [ ] Encryption
    - [ ] Windows Hardening
    - [ ] Mobile Hardening
    - [ ] Secure Communication
    - [ ] Threat Model and Intro(?)
    - [x] Slides
    - [ ] Network Hardening
- 
## Download Template
1. Graphical Option: Use the Download Button Above
1. Terminal Option (Recommended): 

```BASH
git clone https://github.com/irregularchat/Counter-Malign-Influence-POI.git
```


## Update Template
You must navigate to be inside the directory poi-development and execute the following command:
```BASH
git pull
```

## Background of Process and Format
This structure was developed after over a year of course development and instruction, with TRADOC Doctrine and the SWCS Course Developer Course referenced. Fair warning, there is a lot of reading.

The structure in this notebook diverts from Doctrine and SWCS Instruction where needed based on the unique unit limitations, requirements, and size of unit training compared to training at a center of excellence (CoE)

### Developing Training (Writing)
Start with "POI Development"  and use the provided "Developer Workbook" to analyze jobs, tasks, and the audience to be trained.

---
### Teaching Developed Training (Reading)
Start with "POI Training" and Find the Lesson Plans, the Audio Visual Content, and the Evaluations and set up a training area accordingly.

## How to Use This Notebook 
### Obsidian 
This markdown structure is best when used with [Obsidian](https://obsidian.md/) and the following plugins: [Settings > Community Plugins > Browse]
1. Advanced Tables
2. LanguageTool Integration (Spellcheck)
3. Dynamic Table of Contents (Table of Contents)

To expand or collapse sections/headers in a note Top Menu > Insert > {"Fold" or “Unfold”}  or configure a keyboard shortcut using the app preferences

### ELM
Training is designed primarily based on the Experiential Learning Model (ELM), taught at SWCS Course Faculty Course, and is a private sector standard.
 
If you have not been to the SWCS Course Faculty Course yet, study the following content:
- [Gagne's Nine Events of Instruction](https://youtu.be/-31fCUQ2htU)
### Academic Hour
50 minutes is an “hour” to allow students to take a 10-minute break or two 5-minute breaks. 

### Templates
Templates can be notes or entire folders. Duplicate templates as needed. 

### Comments
Comments are between percent symbols (\%%) and may describe. %%This is an inline comment%%

1. Why something is included, excluded, or modified 
2. How to properly use a section
%%This is a comment which... 

...is...
Comments can be single-line or multi-line%%
### Tags
#Knowledge, #Skills, #Resources, and #SupportingTasks should be added as tags to allow for quick sorting and linking

## Notes for Instructors

### NOTES
NOTE is used when an instructor is supposed to perform an action or deliver instruction to students. 

### Links
Pages, Directories, and Files can be linked directly or using relative path formatting. Adding an "!" will embed the page when using obsidian.
![Linked Item Name](./)
or 
[Linked Item Name](./)


### Paraphrasing
> Quote Brackets are used to show the instructor what needs to be paraphrased; a note will also provide this guidance


### Verbatim Quotes and Code
```md
Code Blocks are used for code 
Code Blocks are also used for verbatim requirements, which should not be paraphrased. The code block allows an instructor to notice quickly and to copy if needed.
```

### Spacing and New Lines

To Create New Lines, especially inside a table - use \<br\>, which will create a line break and continue typing. 

Creating a Line Break with a Line can help when sorting content. Use three (3) - in a single line to create a line break such as this:

### Moving to Slides
`##### SLIDE`  should be used to show movement to a new slide. This will allow collapsing and expanding slide instructions to be represented on the table of contents.

---

Spacing and newlines can cause differences in how Obsidian renders markdown. It is essential to include a new line after a "---" line break for proper rendering. 

## Troubleshooting

### sed on MacOS
- Problem: sed for Mac is missing some options which limit cross-compatibility when replacing a string. 
- Solution: Install gnu-sed and map the PATH as needed. `brew install gnu-sed`

### Replace a string in all documents 
in the directory and sub-directories at once. This action should be its own commit to undo any unwanted changes easily. 
- Solution: 
```BASH
grep -RiIl 'Original_String';sleep 5;grep -RiIl 'Original_String' | xargs sed -i 's/Original_String/Replacement_New_String/g'
```

How to Use? Replace Original_String and Replacement_New_String above and input into Terminal inside the desired directory. 
[source](https://www.internalpointers.com/post/linux-find-and-replace-text-multiple-files)

### Run Git Commands on Multiple Directories
- Problem: With multiple git clones, it can be easy to forget which directories need to be updated using `git pull`
- The solution, finding ./git and run the git command on the enclosing directory
```BASH
find . -name .git -print -execdir git pull \;
```
