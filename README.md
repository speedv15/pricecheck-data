# Price Check reference prices

Weekly grocery reference prices for the Northeast US, published for the Price Check iOS app.
Generated automatically every Saturday; don't edit by hand.

**File:** [`v1/baseline-prices.json`](https://speedv15.github.io/pricecheck-data/v1/baseline-prices.json)

## Sources
- **USDA AMS** weekly grocery store feature activity reports (advertised sale prices, Northeast
  region), via the [MyMarketNews API](https://mymarketnews.ams.usda.gov/). Rolling 12 weeks.
- **U.S. Bureau of Labor Statistics** average retail prices (regular prices, Northeast,
  area 0100). Latest 3 months.

Both are U.S. government works in the public domain. This project is not affiliated with or
endorsed by USDA or BLS.

## Format
- Prices are **strings** (`"24.99"`), to keep exact decimal values.
- Dates are calendar days (`yyyy-MM-dd`).
- **`v1/` only ever gains fields.** A change that would break existing app versions goes in a
  new `v2/` folder, published alongside `v1/` until old versions are gone.
