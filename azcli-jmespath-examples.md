---
description: Examples of using JMESPath in the `-query parameter
---

# AZCLI JMESPath Examples

```text
az ad group list --query "[?contains(displayName,'Ma')] | \
[].{GROUPNAME:displayName}" -o table
```

