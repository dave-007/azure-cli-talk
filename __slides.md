---
marp: true
theme: uncover
_class: invert

# Your slide deck

Start writing!
---
# Azure CLI Talk

## For CloudSkills Community

### david@cobbinfotech.com
<!-- todo: complete cit site --> 

---

# Who's Dave?

## - Consultant & Technical Instructor

## - Previously: web developer, accidental dba, intentional dba, system administrator, cloud engineer

## - Microsoft Certified Trainer since 2002, focused on SQL, now on Azure

## - Lots of certifications for Microsoft, Azure & AWS

## - Goal to have a level 1/10 knowledge of most of Azure, with areas 5-8/10.
### - Leveraging Azure CLI and Azure PowerShell is key to grokking and working with these features.
---

# Goals for this talk

- Show how azcli is a **fundamental** tool to learn Azure and become an effective cloud builder
- Equip you with tools to grasp and become effective with azcli quickly
- Convince you to learn by coding azcli and sharing with the CS community via GitHub


---

# Overview

1. Basics: Introduction to Azure CLI Syntax
2. Context: Where CLI fits in your cloud toolbox
3. Tools: Use these to learn faster
4. Challenge: Learn by doing. Code walks
<!-- class: gaia-->



---

<!-- class: uncover invert-->

# uncover + invert

---

# Azure CLI Basics

---

## Azure CLI History

- Formerly XPlat CLI (written in NodeJs)
- Written in Python

---

# Context

## Key Points
- Azure API is THE interface TO Azure, it improves as Azure improves.
  - All cloud tools (Portal, shell, programming, PowerShell & CLI) work against that API
  - azcli is arguably the simplest interface to Azure API
- azcli works on the OS and shell of your choice, including PowerShell
- azcli useful from the PowerShell shell, and alongside AZ PowerShell Modules?

---

## Azure's API

---

## Process of improvement of Azure CLI Commands

### Version history

### Extension (Preview) -> Extension -> Command (Preview) -> Command

```mermaid

graph LR

Extension (Preview) --> Extension --> Command (Preview) --> Command

```

---

## azcli - Shell tradeoffs

### I prefer PowerShell/pwsh over bash or other Linux shells

#### Variables, loops, JSON handling easier for me

#### However awscli, based on python, doesn't support tab completion in pwsh shell [github thread](https://github.com/Azure/azure-cli/issues/2324)

---

##

---

##

---


# Tools

1. -h
2. az interactive
3. az browse
4. jpterm
5. AZCLI VSCode Extension


---

# Challenge
