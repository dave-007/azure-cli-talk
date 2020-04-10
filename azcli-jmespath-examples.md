---
description: Examples of using JMESPath in the `-query parameter
---

# Using --query,  JMESPath Examples



```text
az ad group list --query "[?contains(displayName,'Ma')] | \
[].{GROUPNAME:displayName}" -o table

az account list-locations --query "[?contains(displayName,'US')] | \
[].[displayName,name,id]"

```

