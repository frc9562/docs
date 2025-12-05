---
title: Tag Note Formating
aliases:
  - How to make an Tag Note
  - Tag Note
created: 2025/12/05
modified: 2025-12-05T11:14:56-05:00
tags:
  - documentation
  - style
draft: false
---
Tag notes are markdown files are stored in the tags folder, and will be display anytime a user click on a tag when using [[quartz]]. They are similarly design in the same way an [[Index Note]].   
## The Purpose of Tag Notes
Tag notes main purpose is to help give more context to the purpose of the tag. It should explain the general topic of the tag, what kind of pages should be tag with it, and some core notes that relate to the tag.

## Creating an Tag Notes
To create an Tag Note, use the **Obsidian Quick Add Plugin** on the side ribbon bar or with  
the **command palette**:

```
QuickAdd: Create Tag Note
```

From there, just enter the name of the tag (all lower case) and the script with create the tag and tag note. The tag note will be created in a unfinished state by default, having the notice and being mark as [[TODO]] in the properties. 
## Writing a Tag Note
The tag note should be split into 2 main section
### Context
This is where the tag is explain. It should include information such as what sort of information can be found in these notes, What [[10 - Sub Team/index|Sub Team(s)]] commonly use this note or what types of programs or tools need this information. It shouldn't be long, no more then 2-3 sentience.
#### Format
The general format for the context could follow this structure:

> The *(TAG)* tag is used when *(THE USE CASE FOR THE TAG)* for the *(SUB TEAM)*. 

Its a little vague in what should be in it but as long as you include some explanation and link it to some other note for more content (such as an sub team), it should be good enough. This also written is stone, other format can work too, if it cover all the same information.
### Key Notes
This section is normally blank on most new tags but as a tag get more use, and a few note start to be seen as commonly relate to that tag (for example the [[git]] tag has the major note about the [[GitHub information]]) Those notes should be manually added to these tags note under the Heading of *Key Notes*. This will help user find important note for topic rather then having to search for it them self. 

## Exceptions to Tag Note
There are some situation where Note Tag are formatted a little differently
### When Tag Note Overlap with Index Note
This can happen when dealing with [[10 - Sub Team/index|Sub Team]] as we have both [[index note]] for each sub team while also having a tag for teach sub team. This can also happen for each [[20 - Seasonal/index|Seasonal]], [[30 - Hardware/index|Hardware]] etc. In all case, these Tag Note could redirect anyone that click onto the tag onto the Index file. 
#### Format
The General format for an redirecting tag note is:

> The *(TAG)* tag is used for any note related to *(SHORT CONTEXT)*. Refer to *(INDEX NOTE)* folder for more information.

## References
[Quartz Documentation on Tag Listing](https://quartz.jzhao.xyz/features/folder-and-tag-listings#tag-listings)