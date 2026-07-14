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

## Get Your Free API Key with 10,000 Queries per Month
https://app.whoisdatacenter.com/sign-up


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


## Example JSON Response

```text
{
  "domain": "marketxy.com",
  "query_time": "2026-07-14 20:59:37",
  "create_date": "2024-10-09",
  "update_date": "2025-07-12",
  "expiry_date": "2034-10-09",
  "domain_registrar_id": "1068",
  "domain_registrar_name": "NAMECHEAP INC",
  "domain_registrar_whois": "whois.namecheap.com",
  "domain_registrar_url": "http://www.namecheap.com",
  "registrant_name": "Redacted for Privacy",
  "registrant_company": "Privacy service provided by Withheld for Privacy ehf",
  "registrant_address": "Kalkofnsvegur 2",
  "registrant_city": "Reykjavik",
  "registrant_state": "Capital Region",
  "registrant_zip": "101",
  "registrant_country": "IS",
  "registrant_email": "226954c46487463d9eee2ab909daafd5.protect@withheldforprivacy.com",
  "registrant_phone": "+354.4212434",
  "registrant_fax": "",
  "phone_id": "3544212434",
  "country_id": "IS",
  "administrative_name": "Redacted for Privacy",
  "administrative_company": "Privacy service provided by Withheld for Privacy ehf",
  "administrative_address": "Kalkofnsvegur 2",
  "administrative_city": "Reykjavik",
  "administrative_state": "Capital Region",
  "administrative_zip": "101",
  "administrative_country": "IS",
  "administrative_email": "226954c46487463d9eee2ab909daafd5.protect@withheldforprivacy.com",
  "administrative_phone": "+354.4212434",
  "administrative_fax": "",
  "technical_name": "Redacted for Privacy",
  "technical_company": "Privacy service provided by Withheld for Privacy ehf",
  "technical_address": "Kalkofnsvegur 2",
  "technical_city": "Reykjavik",
  "technical_state": "Capital Region",
  "technical_zip": "101",
  "technical_country": "IS",
  "technical_email": "226954c46487463d9eee2ab909daafd5.protect@withheldforprivacy.com",
  "technical_phone": "+354.4212434",
  "technical_fax": "",
  "billing_name": "",
  "billing_company": "",
  "billing_address": "",
  "billing_city": "",
  "billing_state": "",
  "billing_zip": "",
  "billing_country": "",
  "billing_email": "",
  "billing_phone": "",
  "billing_fax": "",
  "name_servers1": "cass.ns.cloudflare.com",
  "name_servers2": "gerald.ns.cloudflare.com",
  "name_servers3": "",
  "name_servers4": "",
  "domain_statuses1": "clientTransferProhibited https://icann.org/epp#clientTransferProhibited",
  "domain_statuses2": "",
  "domain_statuses3": "",
  "domain_statuses4": "",
  "dns": "unsigned",
  "response_time_ms": 1014.96
}
```

## Credits

Each Live WHOIS Lookup uses 5 credits.

## For Support
https://whoisdatacenter.com/contact-us/


## Official Documentation

https://whoisdatacenter.com/api-docs/#live-whois-lookup

## About WhoisDataCenter

WhoisDataCenter provides WHOIS data, historical WHOIS records, reverse WHOIS lookup, newly registered domain feeds, updated domain feeds, expired domains, expiring domains, and other domain intelligence APIs.

Website: https://whoisdatacenter.com


