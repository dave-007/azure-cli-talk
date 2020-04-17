---
description: Azure CLI Talk Outline
---

# Outline

* Intro
* Goals of This Talk
  * Introduction to Azure CLI
  * Code Walk thru demos
  * **Community Code Walk Challenge**
* What is AZCLI
  * Disambiguate OS,terminal,shell,console, executable, module
  * Another layer to work against Azure API [6 year old blog post](https://docs.microsoft.com/en-us/archive/blogs/mast/learning-azure-service-management-rest-api-through-powershell-and-azure-cli-tools)
* Installation
  * Cross platform
    * For Windows, Use Chocolatey 🤩
	 * `choco install azcli`
	* Or Scoop
	* scoop install azure-cli
	* Included in Azure Cloud Shell
	Where does AZCLI tool fit into your DevOps toolbox?
	* Bash shell versus PowerShell with AZ
  * AZ PowerShell and AZ CLI is not an either/or, it's an AND choice
* Why AZCLI and AZ PowerShell are better together
  * Features unique to AZCLI
    * Talk about teams behind PS and CLI modules
      * Separate cadences, separate functionality
      * Examples
        * AZ ACI BUILD
        * AZ EXTENSION...
  * Tradeoffs between Bash and Pwsh
    * No autocomplete in Pwsh, Bash only! (can use az interactive)
	Development process of the AZCLI
	* ...
	* Command Modules
	* Move from *-preview to part of CLI (See extensions)
	 * Example PY code showing KeyVault change from preview to part of CLI [link] (https://github.com/Azure/azure-cli/blob/8adf97355a605d147afc26f6c1b6f6afb6651c2f/src/azure-cli/azure/cli/command_modules/keyvault/__init__.py)
	DEMOS
* az basics
* az interactive
* az rest (?)
* Handling JSON output
  * JMESPath / the 'bash' way
  * Query demos
    * columns
    * filters
  * ConvertFrom-JSON / the 'pwsh' way
* Extensions
  * Python Wheels
  * az extension list
* Related Tools
  * VSCode
    * Extensions
      * ms-vscode.azurecli
  * AzBrowse
    * Installation
  
      ```bash
      scoop bucket add azbrowse https://github.com/lawrencegripper/scoop-bucket.git
      scoop install azbrowse
      ```

* Identity Options
  * Service account
  * Machine account (demo via SSH)
* Using AZCLI DevOps extension
  * Demo
* Azure DevOps CLI Task
* Azure Pipelines [Demo on Docs](https://docs.microsoft.com/en-us/azure/devops/pipelines/create-first-pipeline-cli?view=azure-devops&tabs=browser)
* References
  * [https://docs.microsoft.com/en-us/cli/azure/popular-articles-using-the-azure-cli?](https://docs.microsoft.com/en-us/cli/azure/popular-articles-using-the-azure-cli?)
  * [https://devblogs.microsoft.com/devops/using-azure-devops-from-the-command-line/](https://devblogs.microsoft.com/devops/using-azure-devops-from-the-command-line/)
  * [https://docs.microsoft.com/en-us/cli/azure/](https://docs.microsoft.com/en-us/cli/azure/)
  * [https://jmespath.org/](https://jmespath.org/)
  * [https://github.com/bbtsoftware/AzureDevOpsPolicyConfigurator](https://github.com/bbtsoftware/AzureDevOpsPolicyConfigurator)
 * [https://docs.microsoft.com/en-us/archive/blogs/mast/learning-azure-service-management-rest-api-through-powershell-and-azure-cli-tools](https://docs.microsoft.com/en-us/archive/blogs/mast/learning-azure-service-management-rest-api-through-powershell-and-azure-cli-tools)
 * [https://dev.to/techwatching/good-bye-azure-portal-welcome-azure-cli-oo2](Dev.To Article by Alexander)

* CHALLENGE
* This looks too hard I don't want to learn it
  * Doing hard things makes later tasks easier
* How would I even start?
  * Code walk through a task or an az command or extension


---


---
description: Azure CLI Talk Outline
---

# Outline

* Intro
* Goals of This Talk
  * Introduction to Azure CLI
  * Code Walk thru demos
  * **Community Code Walk Challenge**
* What is AZCLI
  * Disambiguate OS,terminal,shell,console, executable, module
  * Another layer to work against Azure API [6 year old blog post](https://docs.microsoft.com/en-us/archive/blogs/mast/learning-azure-service-management-rest-api-through-powershell-and-azure-cli-tools)
* Installation
  * Cross platform
    * For Windows, Use Chocolatey 🤩
	 * `choco install azcli`
	* Or Scoop
	* scoop install azure-cli
	* Included in Azure Cloud Shell
	Where does AZCLI tool fit into your DevOps toolbox?
	* Bash shell versus PowerShell with AZ
  * AZ PowerShell and AZ CLI is not an either/or, it's an AND choice
* Why AZCLI and AZ PowerShell are better together
  * Features unique to AZCLI
    * Talk about teams behind PS and CLI modules
      * Separate cadences, separate functionality
      * Examples
        * AZ ACI BUILD
        * AZ EXTENSION...
  * Tradeoffs between Bash and Pwsh
    * No autocomplete in Pwsh, Bash only! (can use az interactive)
	Development process of the AZCLI
	* ...
	* Command Modules
	* Move from *-preview to part of CLI (See extensions)
	 * Example PY code showing KeyVault change from preview to part of CLI [link] (https://github.com/Azure/azure-cli/blob/8adf97355a605d147afc26f6c1b6f6afb6651c2f/src/azure-cli/azure/cli/command_modules/keyvault/__init__.py)
	DEMOS
* az basics
* az interactive
* az rest (?)
* Handling JSON output
  * JMESPath / the 'bash' way
  * Query demos
    * columns
    * filters
  * ConvertFrom-JSON / the 'pwsh' way
* Extensions
  * Python Wheels
  * az extension list
* Related Tools
  * VSCode
    * Extensions
      * ms-vscode.azurecli
  * AzBrowse
    * Installation
  
      ```bash
      scoop bucket add azbrowse https://github.com/lawrencegripper/scoop-bucket.git
      scoop install azbrowse
      ```

* Identity Options
  * Service account
  * Machine account (demo via SSH)
* Using AZCLI DevOps extension
  * Demo
* Azure DevOps CLI Task
* Azure Pipelines [Demo on Docs](https://docs.microsoft.com/en-us/azure/devops/pipelines/create-first-pipeline-cli?view=azure-devops&tabs=browser)
* References
  * [https://docs.microsoft.com/en-us/cli/azure/popular-articles-using-the-azure-cli?](https://docs.microsoft.com/en-us/cli/azure/popular-articles-using-the-azure-cli?)
  * [https://devblogs.microsoft.com/devops/using-azure-devops-from-the-command-line/](https://devblogs.microsoft.com/devops/using-azure-devops-from-the-command-line/)
  * [https://docs.microsoft.com/en-us/cli/azure/](https://docs.microsoft.com/en-us/cli/azure/)
  * [https://jmespath.org/](https://jmespath.org/)
  * [https://github.com/bbtsoftware/AzureDevOpsPolicyConfigurator](https://github.com/bbtsoftware/AzureDevOpsPolicyConfigurator)
 * [https://docs.microsoft.com/en-us/archive/blogs/mast/learning-azure-service-management-rest-api-through-powershell-and-azure-cli-tools](https://docs.microsoft.com/en-us/archive/blogs/mast/learning-azure-service-management-rest-api-through-powershell-and-azure-cli-tools)
 * [https://dev.to/techwatching/good-bye-azure-portal-welcome-azure-cli-oo2](Dev.To Article by Alexander)

* CHALLENGE
* This looks too hard I don't want to learn it
  * Doing hard things makes later tasks easier
* How would I even start?
  * Code walk through a task or an az command or extension
