# Live WHOIS Lookup API

Get fresh WHOIS data directly from the registry in real time.

The Live WHOIS Lookup API returns the newest available WHOIS information for a domain directly from the registry.

## Endpoint

```http
GET https://api-v1.whoisdatacenter.com/api/v2/domain/whois/live
```

## Parameters

| Parameter | Required | Description |
|---|---|---|
| domain | Yes | Domain name to look up, such as `yahoo.com` |
| format | No | Response format: `json`, `xml`, or `csv`. Default is `json` |

## Example Request

```bash
curl -X GET "https://api-v1.whoisdatacenter.com/api/v2/domain/whois/live?domain=yahoo.com" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Accept: application/json"
```

## Authentication

Use your API key as a Bearer token:

```text
Authorization: Bearer YOUR_API_KEY
```

Never publish your real API key on GitHub or in public code.

## Example API URL

```text
https://api-v1.whoisdatacenter.com/api/v2/domain/whois/live?domain=yahoo.com
```

## Response Formats

The API supports:

- JSON
- XML
- CSV

JSON is used by default.

Example with XML:

```text
https://api-v1.whoisdatacenter.com/api/v2/domain/whois/live?domain=yahoo.com&format=xml
```

Example with CSV:

```text
https://api-v1.whoisdatacenter.com/api/v2/domain/whois/live?domain=yahoo.com&format=csv
```

## Credits

Each Live WHOIS Lookup uses 5 credits.

## Official Documentation

https://whoisdatacenter.com/api-docs/#live-whois-lookup

## About WhoisDataCenter

WhoisDataCenter provides WHOIS data, historical WHOIS records, reverse WHOIS lookup, newly registered domain feeds, updated domain feeds, expired domains, expiring domains, and other domain intelligence APIs.

Website: https://whoisdatacenter.com
