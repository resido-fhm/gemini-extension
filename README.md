# Ferienhausmiete.de – Gemini CLI extension

Search privately owned holiday homes and apartments on [Ferienhausmiete.de](https://www.ferienhausmiete.de) directly from Gemini CLI / Antigravity: region lookup, dated searches with exact total stay prices, listing details and day-by-day availability. No account, no API key, no booking fees for guests.

## Install

```
gemini extensions install https://github.com/ferienhausmiete/gemini-extension
```

## Example prompts

- "Find a holiday home on the Baltic Sea for 4 people from 27 March to 3 April, dogs allowed, with sauna – with the total price."
- "Was kostet eine Ferienwohnung in Binz über Silvester für 2 Personen?"
- "Show me listings with best-price guarantee in the Black Forest under €100 per night."

## What it connects to

Remote MCP server `https://mcp.ferienhausmiete.de/` (Streamable HTTP, read-only, no authentication). Four tools: `autocomplete_regions`, `search_accommodations`, `get_accommodation`, `get_accommodation_availability`. Responses in de, en, fr, pl, it, es, nl, hr.

## Privacy and terms

Only the search parameters you type (region, dates, guests, amenities) are sent to the server; no account or conversation data. Terms: https://www.ferienhausmiete.de/l/mcp-nutzungsbedingungen/ · Privacy: https://www.ferienhausmiete.de/datenschutz.php · Contact: support@ferienhausmiete.de

Operated by resido GmbH, Berlin.
