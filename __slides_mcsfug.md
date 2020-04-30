---
marp: true
theme: uncover
_class: invert

# Your slide deck

Start writing!
---



---

# Azure CLI Talk

## For Microsoft Cloud South Florida User Group | MCSFUG

### David Cobb
### david@davidcobb.net

---

# Intro

### - Consultant & Technical Instructor

### - Career path: helpdesk, web developer, dba, system administrator, cloud engineer

### - Microsoft Certified Trainer since 2002, was focused on SQL, now focused on Azure. Certifications for Microsoft SQL, Azure & two for AWS

### - Generalist. My goal is baseline knowledge of most of Azure, with deeper study in a few areas of interest (SQL/Data/ML/AI).

---

# Goals for this talk

- Getting started with of Azure CLI **(Command Line Interface, aka AZCli )** as part of your Azure toolbox. 

- Share tools and techniques in the shell with Azure CLI

- Explore Azure CLI commands, beginning with the fundamentals useful for AZ-104 (Storage, VMs, Networking)

- Discover interesting preview Azure CLI commands and extensions

- Challenge you to learn Azure CLI by coding and sharing with the CS community via GitHub

---
# Installing & Running AZCLI
###  Azure CLI is written in Python, so it's cross platform, runs in Windows, Linux, MacOS
### Is open source under MIT License
### Has many ways to install ([docs](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)) 
### Works* on your choice of shell: bash, zsh, pwsh, etc...

## David's shell of choice to run AZCLI is _PowerShell 7_ (pwsh) *

##### * _Aspects of Azure CLI like `--query` are not perfectly cross platform yet.._
---

# Shell Considerations

## What's your shell?

### Practice makes (better). It's a time investment to become proficient in a shell, this pays off in increasing effectiveness, especially in the cloud.

### See [Tips for using Azure CLI effectively](https://github.com/Azure/azure-cli/blob/dev/doc/use_cli_effectively.md) for help with common challenges that arise with shell scripting using this tool.

### We will use different shells that each have their strengths, but the focus of this talk is not the shell but Azure CLI.


---

# Using VSCode? You should be!

## Check out the 'Azure CLI Tools' extension

```ps

code --install-extension ms-vscode.azurecli

```

## Works with the shell of your choice

![VSCode shell choices](https://i.imgur.com/4xCD1yG.png)

---

# Azure CLI Basics

### Start with Azure API

### Basic Syntax

### First Commands

### Get Interactive

### Dealing with JSON

---

# Azure's API

### As the Underlying control plane for all of Azure, the API has a HUGE, RAPIDLY EVOLVING scope
- [Azure API docs](https://docs.microsoft.com/en-us/rest/api/azure/) 
- [Azure API releases on github](https://github.com/Azure/azure-rest-api-specs/releases)

### Azure CLI is also updated frequently
- [AZCLI release notes](https://docs.microsoft.com/en-us/cli/azure/release-notes-azure-cli)
- [AZCLI issues tracker](https://github.com/Azure/azure-cli/issues)

### Compare to Azure PowerShell's update frequency
- [Azure PowerShell release notes](https://docs.microsoft.com/en-us/powershell/azure/release-notes-azureps)
- [Azure PowerShell issues tracker](https://github.com/azure/azure-powershell/issues)

---

# DAVE'S STANDARD 
# _'CLOUD BASED BLEEDING EDGE TOOLS'_
# WORD OF CAUTION 

## Using many tools in development or preview, some of these demos may not work!
#### We can learn a lot troubleshooting things that break!
#### Even so, be wary of dragons (or bugs).

---

# Demo Azure API

## Use the [Azure Resource Explorer](https://resources.azure.com/) to work against Azure API after authenticating to your Azure account.

### But why use a web page when you can use Lawrence Gripper's [AzBrowse](https://github.com/lawrencegripper/azbrowse)?

#### Add **az browse** command to azcli using Noel Bundick's [custom azcli extension](https://github.com/noelbundick/azure-cli-extension-noelbundick)

```
az extension add --source https://github.com/noelbundick/azure-cli-extension-noelbundick/releases/download/v0.0.17/noelbundick-0.0.17-py3-none-any.whl
```


---

## Azure CLI Basic Syntax & First Commands

### Arguments syntax
-  Start with az -h
-  All params start with two hyphens (--help),most common arguments have a one hyphen short format (-h)
-  After `az login`, start with `az group -h` to work with your resource groups and get familiar with Azure CLI syntax
-  You can save work later by setting some smart defaults with `az configure`
---

### Global Arguments work for most commands

```
    --debug            : Increase logging verbosity to show all debug logs.
    --help -h          : Show this help message and exit.
    --only-show-errors : Only show errors, suppressing warnings.
    --output -o        : Output format.  Allowed values: json, jsonc, none, table, tsv, yaml, yamlc.
                         Default: jsonc.
    --query            : JMESPath query string. See http://jmespath.org/ for more information and
                         examples.
    --subscription     : Name or ID of subscription. You can configure the default subscription
                         using `az account set -s NAME_OR_ID`.
    --verbose          : Increase logging verbosity. Use --debug for full debug logs.
```


---

# Get Interactive

## az interactive

### explore commands with intellisense

### embedded documentation

### examples with step by step tutorials

---

# Dealing with JSON

## --query & JMESPath

## [jmespath-terminal / jpterm](https://github.com/jmespath/jmespath.terminal)

## Why not PowerShell & ConvertFrom-JSON?

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
-----------------------> CLI Command (Preview) 
----------------------------> CLI Command (Released)


Example, [az keyvault command was previously an extension in preview](https://github.com/Azure/azure-cli/blob/8adf97355a605d147afc26f6c1b6f6afb6651c2f/src/azure-cli/azure/cli/command_modules/keyvault/__init__.py)

---

# Explore some Azure CLI commands and extensions

---

# Your Turn to Explore Azure Cli 

## Code-Walk Challenge!
---

# Q & A

---