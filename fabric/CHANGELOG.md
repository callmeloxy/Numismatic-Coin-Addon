# Changelog

## 1.0.1

### Summary

Polish update improving Numismatic Coin Addon integration with the Numismatic Overhaul purse UI.

### Fixed

- Fixed Emerald and Diamond coin stack visuals not updating correctly
- Fixed Diamond Coin stack rendering when using a custom max stack size
- Fixed the purse tooltip displaying large Gold values instead of properly splitting values into Diamond, Emerald, Gold, Silver, and Bronze
- Fixed several purse UI display issues caused by the extended currency layout
- Fixed missing default config handling for Diamond Coin max stack size

### Added

- Added extended purse display support for Diamond and Emerald values
- Added Diamond and Emerald entries to the purse popup menu
- Added support for extracting Diamond and Emerald coins directly from the purse popup
- Added default config file for Numismatic Coin Addon
- Added configurable Diamond Coin max stack size

### Changed

- Changed the purse value display to use the full extended currency order:
  - Diamond
  - Emerald
  - Gold
  - Silver
  - Bronze

### Improved

- Improved Emerald and Diamond coin textures to better match the Numismatic Overhaul visual style
- Improved stacked coin visuals for Emerald and Diamond coins
- Improved the extended purse popup texture for better consistency with Numismatic Overhaul
- Improved the right-side coin column of the extended purse popup so it appears cleaner and less visually cut
- Improved command and config consistency after the final mod rename to Numismatic Coin Addon

### Notes

- Diamond Coin max stack size defaults to 21 for safer compatibility
- The Diamond Coin max stack size can be changed in `config/NumismaticCoinAddon/config.json`
- Changing the Diamond Coin max stack size requires a full game restart
- Values above 21 for Diamond Coin max stack size may increase the risk of overflow issues in some currency-related code paths

## 1.0.0

### Summary

Initial release of Numismatic Coin Addon, adding two higher-tier coins above Gold for Numismatic Overhaul.

### Added

- Added Emerald Coin
- Added Diamond Coin
- Added support for Numismatic Overhaul currency values
- Added compatibility with Numismatic CheesePurse
- Added stacked visual models for Emerald Coin and Diamond Coin
- Added configurable Diamond Coin max stack size
- Added default config file generation
- Added `/nca` command
- Added `/numismaticaddon` command alias
- Added coin conversion commands

### Changed

- Changed the currency progression with a new high-tier structure:
  - 100 Gold = 1 Emerald
  - 100 Emerald = 1 Diamond

### Improved

- Improved Emerald and Diamond coin textures to match the visual style of Numismatic Overhaul coins
- Improved Diamond Coin stack-size handling through config support
- Improved command naming so it matches the final mod name

### Notes

- Default Diamond Coin max stack size is set to 21 for safer compatibility with Numismatic Overhaul and CheesePurse
- Increasing the Diamond Coin stack size above 21 may expose overflow issues in some currency-related code paths
