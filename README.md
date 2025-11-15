# AREDN Service Browser

AREDN Service Browser is a single-page, client-side tool for exploring services
exposed on Amateur Radio Emergency Data Network (AREDN) mesh nodes. It fetches the
`/a/sysinfo` (or legacy `cgi-bin/sysinfo.json`) endpoint directly from your
browser and renders hosts, services (remote and local), links, and link quality 
monitor details in a readable format.

## Features

- **Dynamic node selection** – By default, queries localnode.local.mesh, but allows selection from discovered mesh nodes, or manually enter a hostname/IP. 
- **Node summary** – Shows the active node, firmware version, API in use, and API version.
- **Hosts overview** – Sorted host tables with live filtering across names and IP addresses.
- **Service grouping** – Services are grouped by explicit `[category]` tags or by URL scheme (e.g., `winlink://`), each with collapsible sections and JSON inspection.
- **Link lists** – Link info and LQM trackers render as clickable lists so you can inspect their raw JSON quickly.
- **JSON inspector** – Click any row to view the formatted JSON payload in a modal dialog for debugging.

## Usage

1. Download this directory to a computer on the AREDN network and open `index.html` directly in your browser . Optionally serve from any web server that is accessible by devices on the AREDN network.

## Development Notes

- All logic lives inside the single `index.html` file.
- Developed almost completely using ChatGPT

## License

This project is released under the [MIT License](LICENSE).

