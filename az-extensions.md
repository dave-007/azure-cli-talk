---
description: >-
  Introduce the AZ CLI extensions functionality. These are analagous to modules
  in PowerShell. Implemented as Python Wheels
  References:
  https://github.com/Azure/azure-cli/tree/master/doc/extensions
---

# az extensions

```ps
az extension list-available -o table

$extensions = az extension list-available | ConvertFrom-JSON
$extensions | Out-GridView 


```

## extensions of interest

- az support
- az resource-graph
- az subscription
  
```ps


```
