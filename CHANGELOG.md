# MK Weed – Changelog

## 1.0.4 – 2026-10-17

### Fixed
- No more "Could not make hard link" warning on start: the models note moved out of the stream folder (docs/models.md)

## 1.0.3 – 2026-10-16

### Fixed
- Two players could harvest or seed the same plant at the same moment
- Watering no longer works for free when the inventory has no room for the split-off can
- Two buyers could both pay for the same lab
- Logging out inside a lab no longer leaves the next character in an empty copy of the world
- A break-in started again at the same door no longer spams the owner and the police
- Shop, dealer and buyer menus work with every target system; pots and tables can no longer open two previews
- Lab laptop props of a second lab are no longer deleted when switching labs; help text is hidden on resource stop
- Plant cards of lab worker pots now sit right on top of the plant instead of a metre higher
- Lab workers no longer stand on buckets or shelves – they pick a free spot on the floor next to their pot

### Changed
- Smoother plant status cards: only changed values are drawn, one message router instead of 16 listeners, shared countdown clock
- Less client load: framework job / loaded checks cached instead of asked every frame, lab state read from a local copy
- Less database load: 10 indexes no query used are removed automatically, dashboard and owner lookups no longer scan whole tables
- Discord logs are batched (no more rate limits) and can never ping anyone
- Smaller, tidier corners in every window

## 1.0.2 – 2026-10-15

### Fixed
- Plant cards of lab worker pots now sit right on top of the plant instead of a metre higher
- Lab workers no longer stand on buckets or shelves – they pick a free spot on the floor next to their pot

### Changed
- Cleaner server console: one ready line with the version on start – details only with Config.Debug
- Warnings and errors now use one consistent, prefixed format
