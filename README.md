# SCM-DD-COLLECTOR

A custom GitHub Action that collect and publish any given action (workflow) result to Datadog.

## Inputs

### `action-name`

**Required** Github Action (workflow) name.

### `sonar-base-url`

**Required** Sonarqube Base URL.

### `datadog-base-url`

**Required** Datadog Base URL.

### `dd-api-key`

**Required** Your DataDog API Key. Get it from your DataDog subscription.

### `dd-application-key`

**Required** Your DataDog Application Key. Get it from your DataDog subscription.

## Example Usage

```yaml
uses: yauritux/gh-dd-collector@v1.0
with:
  action-name: release
  datadog-base-url: ${{ secrets.DD_BASE_URL }}
  dd-api-key: ${{ secrets.DD_API_KEY}}
  dd-application-key: ${{ secrets.DD_APPLICATION_KEY }}
```
