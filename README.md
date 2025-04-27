# <img width="24px" src="./logo.png" alt="Wrestlarr"></img> Wrestlarr

[![Build Status](https://github.com/<org>/Wrestlarr/actions/workflows/ci.yml/badge.svg)](https://github.com/<org>/Wrestlarr/actions)
[![Coverage Status](https://coveralls.io/repos/github/<org>/Wrestlarr/badge.svg?branch=main)](https://coveralls.io/github/<org>/Wrestlarr?branch=main)
[![Docker Pulls](https://img.shields.io/docker/pulls/<org>/wrestlarr.svg)](https://hub.docker.com/r/<org>/wrestlarr)
[![License](https://img.shields.io/github/license/<org>/Wrestlarr.svg)](LICENSE)
[![Backers on Open Collective](https://opencollective.com/Wrestlarr/backers/badge.svg)](#backers)
[![Sponsors on Open Collective](https://opencollective.com/Wrestlarr/sponsors/badge.svg)](#sponsors)

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
   git clone https://github.com/<org>/Wrestlarr.git
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

All contributions are welcomed and reviewed according to our [code of conduct](CODE_OF_CONDUCT.md). Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on submitting issues and pull requests.

<a href="https://github.com/<org>/Wrestlarr/graphs/contributors">
  <img src="https://opencollective.com/Wrestlarr/contributors.svg?width=890&button=false" alt="Contributors" />
</a>

## Supporters

Thank you to our backers and sponsors for making this project possible.
[Become a sponsor or backer](https://opencollective.com/Wrestlarr) to support ongoing development.

### Mega Sponsors

[![Mega Sponsors](https://opencollective.com/Wrestlarr/megasponsors/badge.svg)](https://opencollective.com/Wrestlarr/contribute/mega-sponsor/checkout)

### Sponsors

[![Sponsors](https://opencollective.com/Wrestlarr/sponsors.svg?width=890)](https://opencollective.com/Wrestlarr/contribute/sponsor/checkout)

### Backers

[![Backers](https://opencollective.com/Wrestlarr/backers/badge.svg)](https://opencollective.com/Wrestlarr/contribute/backer/checkout)

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.