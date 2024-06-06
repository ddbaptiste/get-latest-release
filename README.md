# Get Latest Release Tag
Get the newest release tag for the current repository

## Usage
```yaml
jobs:
  job-name:
    runs-on: ubuntu-latest
    steps:

      - uses: actions/checkout@v3

      - name: Get Latest Release Version
        id: get-latest-release
        uses: ddbaptiste/get-latest-release@1.0.0

      - name: Print Latest Release
        run: echo ${{ steps.fetch-latest-release.outputs.latest-release }}
```
