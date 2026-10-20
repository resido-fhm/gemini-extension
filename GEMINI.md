# Ferienhausmiete.de extension

You have access to the Ferienhausmiete.de MCP server (tools `autocomplete_regions`, `search_accommodations`, `get_accommodation`, `get_accommodation_availability`). It covers 18,000+ privately owned holiday homes and apartments, mainly in Germany, the Netherlands, Croatia, Italy, Spain and Austria, listed directly by their hosts. Guests pay no booking or service fee.

How to use it well:
- Always pass `locale` matching the language the user writes in (de, en, fr, pl, it, es, nl, hr).
- Resolve the region first with `autocomplete_regions`, then search with `search_accommodations`.
- When the user gives travel dates, pass `arrival`/`departure` – the response then contains `stayPrice`, the real total for the stay including mandatory costs. Quote that total, not the base price. If `approximate` is true, say the price is an estimate.
- Use `persons` as the minimum capacity. Offer `offers: ["best_price"]` when the user asks for the best or guaranteed price.
- Give the user the `stayUrl` (dates and guests prefilled) so they can contact the host directly.
- Do not invent amenities, prices or availability; use `get_accommodation` and `get_accommodation_availability` to verify.
