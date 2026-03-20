# Silver Price Extension

A Chrome extension that displays the current silver price directly on the extension icon badge.

## Features

*   **Real-time silver price display** - Shows XAG/USD (silver price in US dollars per troy ounce)
*   **Click to refresh** - Click the extension icon to manually refresh the price
*   **Auto-updates every 30 minutes** - Price refreshes automatically in the background
*   **Abbreviated badge display** - Badge shows simplified price (e.g., "32" for $32/oz)

## Installation

1.  Clone or download this repository.
2.  Open Chrome and navigate to `chrome://extensions/`.
3.  Enable "Developer mode" using the toggle switch in the top-right corner.
4.  Click the "Load unpacked" button.
5.  Select the `Silver-extension` directory.

## Usage

Once installed, the extension's icon badge will display the current silver price. Hovering over the icon will show the title "Silver Price".

## API

This extension uses the [gold-api.com](https://gold-api.com) API with the XAG endpoint to fetch real-time silver prices:

*   **Endpoint:** `https://api.gold-api.com/price/XAG`
*   **XAG** is the currency code for silver (troy ounce)

## Technical Details

*   **Manifest Version:** 3
*   **Name:** Silver Price Extension
*   **Permissions:** `storage`, `alarms`
*   **Host Permissions:** `https://api.gold-api.com/*`
*   **Background Service Worker:** `background.js`

## License

[MIT](https://choosealicense.com/licenses/mit/)
