### ⚠ THIS IS STILL A WORK IN PROGRESS ⚠

# crowdin-action

GitHub Action to interact with the Crowdin CLI

## Examples

### Uploading Source Files on Push

```yaml
on: push
name: upload sources to crowdin
jobs:
  upload:
    name: upload
    runs-on: ubuntu-latest
    steps:
    - name: checkout
      uses: actions/checkout@v1
    - name: upload
      uses: SwitchbladeBot/crowdin-action@v1
      with:
        args: upload sources
```
