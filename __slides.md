---
marp: true
theme: uncover
_class: invert

# Your slide deck

Start writing!
---
<!-- todo: complete cit site --> 

---

# Azure CLI Talk

## For CloudSkills Community

### david@davidcobb.net

 
---

---


# Who's David?

### - Consultant & Technical Instructor

### - Previously: web developer, dba, system administrator, cloud engineer

### - Microsoft Certified Trainer since 2002, was focused on SQL, now focused on Azure

### - Lots of certifications for Microsoft, Azure & two for AWS

### - Generalist. My goal is baseline knowledge of most of Azure, with deeper study in a few areas of interest (SQL/Data/ML/AI).

---

# Goals for this talk

- Overview of Azure CLI **(Command Line Interface, aka azcli)** as part of your Azure toolbox

- Share tools and techniques for Azure CLI that make it easier to learn and build in Azure

- Explore basic Azure CLI commands, including the fundamentals useful for AZ-104 (Storage, VMs, Networking)

- Discover interesting preview Azure CLI commands and extensions

- Challenge you to learn Azure CLI by coding and sharing with the CS community via GitHub


---
# Where can I run Azure CLI?

## AZCLI is cross platform, runs in Windows, Linux, MacOS

## AZCLI works on your choice of shell (even CMD.exe)

## David's shell of choice is PowerShell7 (pwsh)


---

# Azure CLI Basics

## Start with Azure API

## Basic Syntax

## First Commands

## Get Interactive

## Dealing with JSON
---

## Azure's API

---

## Basic Syntax & First Commands

### Parameter syntax

### -h

### Common parameters
- -o, --debug, ...

---

# Get Interactive

## az interactive

---

## Dealing with JSON

### --query & JMESPath

### jpterm

### Why not PowerShell?


---

## Discovering AZCLI Commands and Extensions

---

## Development Process of Azure CLI Commands

### The Azure CLI team shares their dev environment setup for interested developers who want to contribute.  [AZDEV project](https://github.com/Azure/azure-cli-dev-tools)

### New functionality seems to go through these stages:
-----> Extension (Development) 
-------------------> Extension (Preview) 
---------------------------------> Extension (Released)
-----------------------------------------------> Command (Preview) 
-------------------------------------------------------------> Command (Released)

### Example: KeyVault code [link](https://github.com/Azure/azure-cli/blob/8adf97355a605d147afc26f6c1b6f6afb6651c2f/src/azure-cli/azure/cli/command_modules/keyvault/__init__.py)

### [Azure CLI Extensions Project on github](https://github.com/Azure/azure-cli-extensions)


---

# Dave's Take

## Key Points
- Azure API is THE interface to Azure, underlying all the cloud  tools (Portal, shell, programming, PowerShell & CLI) work against that API
- Azure CLI works on the OS and shell of your choice, including PowerShell
- Azure CLI is arguably the simplest interface to Azure API
- Azure CLI is perhaps the best way to keep up with new Azure capabilities
- **Let's learn and share what we learn as a community**

---

---
# Q&A

### How does Azure CLI compare with Azure PowerShell?

### What about ARM Templates, or IaC tools like Terraform or Pulumi?

---

## azcli - Shell tradeoffs

### I prefer PowerShell/pwsh over bash or other Linux shells

#### Variables, loops, JSON handling easier for me

#### However awscli, based on python, doesn't support tab completion in pwsh shell [github thread](https://github.com/Azure/azure-cli/issues/2324)

---

## Compare AZCLI to AZ POWERSHELL

### Azure PowerShell Modules Listing [docs](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md)

---

##

---


# More AZCLI Tools

1. az browse
2. 
3. AZCLI VSCode Extension

---
# JSON & JMESPath References

## [Azure Docs - Query Azure CLI command output](https://docs.microsoft.com/en-us/cli/azure/query-azure-cli)
## [Neil Peterson blog post](https://techcommunity.microsoft.com/t5/itops-talk-blog/how-to-query-azure-resources-using-the-azure-cli/ba-p/360147)


---

# Challenge

---

Extra stuff


---

---

# Overview

1. Basics: Introduction to Azure CLI Syntax
2. Context: Where CLI fits in your cloud toolbox
3. Tools: Use these to learn faster
4. Challenge: Learn by doing. Code walks
<!-- class: gaia-->

---

## Azure CLI History

- Formerly XPlat CLI (written in NodeJs)
- Rewritten in Python
- Updated several times a year, see version history 

---