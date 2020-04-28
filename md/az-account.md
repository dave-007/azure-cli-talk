# az account set -s NAME_OR_ID

## service principal

##  interesting demo az login --identity? managed identities
### https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-sign-in

### access token info https://mikhail.io/2019/07/how-azure-cli-manages-access-tokens/

```bash

token=$(az account get-access-token | jq -r .accessToken)

```
