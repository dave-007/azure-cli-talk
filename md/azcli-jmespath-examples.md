---
description: Examples of using JMESPath in the `-query parameter
---

refer: https://docs.microsoft.com/en-us/cli/azure/query-azure-cli


# Using --query,  JMESPath Examples



```text
az ad group list --query "[?contains(displayName,'Ma')] | \
[].{GROUPNAME:displayName}" -o table

az account list-locations --query "[?contains(displayName,'US')] | \
[].[displayName,name,id]"

```

