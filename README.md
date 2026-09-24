# <img width="24px" src="./logo.png" alt="Wrestlarr"></img> Wrestlarr

[![License](https://img.shields.io/github/license/ericrosenberg1/Wrestlarr.svg)](LICENSE.md)

Wrestlarr is a personal video recorder (PVR) tailored for professional wrestling content. It monitors multiple feeds for new events and episodes, downloads and organizes files, and upgrades quality when better formats become available.

## Getting Started

### Prerequisites

- Docker & Docker Compose
- .NET 6.0 SDK (or later)
- Node.js & npm (for the web UI)
- PostgreSQL or SQLite
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ericrosenberg1/Wrestlarr.git
   cd Wrestlarr
   ```
2. Copy the example configuration and update credentials:
   ```bash
   cp appsettings.json.example appsettings.json
   ```
3. Launch with Docker Compose:
   ```bash
   docker-compose up -d
   ```
4. Open your browser to `http://localhost:8081` to access the web UI.

### Running Tests

- **Server tests**:
  ```bash
  cd src/Wrestlarr.Server
  dotnet test
  ```
- **UI tests**:
  ```bash
  cd src/Wrestlarr.UI
  npm test
  ```

## Features

- Support for WWE, AEW, NJPW, Impact, ROH and other promotions
- Automatic detection and download of new events
- Library scan to identify and fetch missing content
- Quality upgrade when superior formats are released
- Integration with SABnzbd, NZBGet, qBittorrent, Transmission
- Customizable renaming schemes
- RESTful API for automation and third-party integrations
- Responsive, mobile-friendly web UI

## Roadmap

- **v0.1 (Alpha)**: Core download, sorting, and rename functionality
- **v0.2 (Beta)**: Multi-promotion support, UI enhancements, plugin framework
- **v1.0**: Official stable release, localization, mobile optimizations
- **v1.x**: Plugin repository, webhooks, authentication, performance tuning

## Contributing

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on submitting issues and pull requests.

<a href="https://github.com/ericrosenberg1/Wrestlarr/graphs/contributors">Contributors</a>

## License

This project is licensed under the GNU General Public License v3.0. See [LICENSE.md](LICENSE.md) for details.