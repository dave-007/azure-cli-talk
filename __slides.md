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

## - Career path: helpdesk, web developer, dba, system administrator, cloud engineer

## - Microsoft Certified Trainer since 2002, was focused on SQL, now focused on Azure. Certifications for Microsoft, Azure & two for AWS

### - Generalist. My goal is baseline knowledge of most of Azure, with deeper study in a few areas of interest (SQL/Data/ML/AI).

---

# Goals for this talk

- Getting started with of Azure CLI **(Command Line Interface, aka azcli)** as part of your Azure toolbox. 

- Share tools and techniques in the shell with Azure CLI

- Explore Azure CLI commands, beginning with the fundamentals useful for AZ-104 (Storage, VMs, Networking)

- Discover interesting preview Azure CLI commands and extensions

- Challenge you to learn Azure CLI by coding and sharing with the CS community via GitHub


---
# Installing & Running AZCLI
## AZCLI ..
###  Is written in Python, so it's cross platform, runs in Windows, Linux, MacOS
### Is open source under MIT License
### Has many ways to install ([docs](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest))
### Works on your choice of shell bash, zsh, etc...even CMD.exe)

## David's shell of choice to run AZCLI is _PowerShell7 (pwsh)_

---

# Shell Considerations

## What's your shell?

### It's a time investment to become proficient in a shell, this pays off in effectiveness with AZCLI or any other command line tool.

### See [Tips for using Azure CLI effectively](https://github.com/Azure/azure-cli/blob/dev/doc/use_cli_effectively.md) for help with common challenges that arise with shell scripting using this tool.

---

# Using VSCode? You should be!

## Check out the Azure CLI Tools extension

```ps

code --install-extension ms-vscode.azurecli

```


---

# Azure CLI Basics

## Start with Azure API

## Basic Syntax

## First Commands

## Get Interactive

## Dealing with JSON
---

# Azure's API

## Underlying control plane for all of Azure. 
## Huge scope, changing rapidly. 
- [Azure API docs](https://docs.microsoft.com/en-us/rest/api/azure/) 
- [releases on github](https://github.com/Azure/azure-rest-api-specs/releases)

## Azure CLI is updated frequently
- [AZCLI release notes](https://docs.microsoft.com/en-us/cli/azure/release-notes-azure-cli)

## Compare to Azure PowerShell's update frequency
- [Azure PowerShell release notes](https://docs.microsoft.com/en-us/powershell/azure/release-notes-azureps)

---

# Demo Azure API

---

# Basic Syntax & First Commands

### Parameter syntax

-  -h
-  ...

### Common parameters
- -o, --debug, ...
- ...
### Demo
---

# Get Interactive

## az interactive

---

# Dealing with JSON

## --query & JMESPath

## jpterm

## Why not PowerShell? :)


---

# Demo AZCLI, JSON & PowerShell

---

# Discovering AZCLI Commands and Extensions

---
# Azure CLI Open Source Projects in GitHub

## [Azure CLI](https://github.com/Azure/azure-cli)
## [Azure CLI Extensions](https://github.com/Azure/azure-cli-extensions)

- [Azure Commands under development](https://github.com/Azure/azure-cli-extensions/tree/master/src)


## [Microsoft Azure CLI Dev Tools (azdev) ](https://github.com/Azure/azure-cli-dev-tools)



---



## Development Process of Azure CLI Commands

-----> Extension (Development) 
------------> Extension (Preview) 
-----------------> Extension (Released)
-----------------------> Command (Preview) 
----------------------------> Command (Released)


Example, [az keyvault command was previously an extension in preview](https://github.com/Azure/azure-cli/blob/8adf97355a605d147afc26f6c1b6f6afb6651c2f/src/azure-cli/azure/cli/command_modules/keyvault/__init__.py)

---

# Explore some Azure CLI commands and extensions

---

# Your Turn to Explore Azure Cli 

## Code-Walk Challenge!
---

# Q & A

---

# Dave's Take

## Key Points
- Azure API is THE interface to Azure, underlying all the cloud  tools (Portal, shell, programming, PowerShell & CLI) work against that API
- Azure CLI works on the OS and shell of your choice, including PowerShell
- Azure CLI is arguably the simplest interface to Azure API
- Azure CLI is perhaps the best way to keep up with new Azure capabilities
- **Let's learn and share what we learn as a community**

---

# End Slides

...Extra Stuff to Follow

---

Questions, 

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

- az browse
- 
- AZCLI VSCode Extension
  - install vscode extension

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