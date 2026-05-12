# Hardening Audit Viewer

A premium, interactive web-based dashboard that transforms your system hardening audit JSON files into an easily digestible visual format.

Developed by **Chuck Talk** as a **Nordheim Online product**.

## Features

- **Local Processing**: Upload your JSON file directly in the browser. No data is sent to any server; everything is processed securely on your local machine.
- **Tabbed Architecture**: Services are automatically grouped into dynamic tabs based on their severity (`UNSAFE`, `EXPOSED`, `MEDIUM`, `OK`).
- **Alphabetical Sorting**: Within each severity level, all cards are alphabetized for quick scanning.
- **Premium Aesthetics**: Features a modern dark-mode theme, smooth animations, and clear color-coding mapped to the exposure risk score.

## How to Use

1. Clone or download this repository.
2. Open `index.html` in any modern web browser.
3. Click the **"Select JSON File"** button at the top of the dashboard.
4. Select your `hardening_audit.json` file.
5. Review your security audit in a human-digestible format.

## Example JSON Format

The viewer expects a JSON array of objects with the following structure:

```json
[
  {
    "unit": "NetworkManager.service",
    "exposure": "7.8",
    "predicate": "EXPOSED",
    "happy": "🙁"
  }
]
```

## License

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the `LICENSE` file for more details.

Copyright (C) 2026 Chuck Talk as a Nordheim Online product.
