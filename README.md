# be-api

## Get token

```sh
az account get-access-token --resource https://purview.azure.net --query accessToken --output tsv
```

## rest-client config

1. Create .vscode/settings.json file
1. Add

```json
{
    "rest-client.environmentVariables": {

        "$shared": {},

        "local": {
            "PURVIEW_NAME": "eiffel-pv",
            "PURVIEW_TOKEN": "COPY TOKEN FROM ABOVE"
        },
    }
}
```
1. Open Palette, search `rest-client: Switch Environment` and select `local`