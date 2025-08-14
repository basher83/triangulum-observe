# Documentation Structure

This document outlines the organization and naming conventions for the `triangulum-observe` repository.

## Repository Structure

```text
triangulum-observe/
├── docs/                    # General documentation and guides
├── reports/                 # Monitoring reports and exports
└── solutions/               # Product-specific configurations and docs
    ├── netdata/            # Netdata-specific content
    ├── zabbix/             # Zabbix-specific content
    └── checkmk/            # CheckMK-specific content
```

## Directory Purposes

### `docs/`
- High-level guides, runbooks, and how-tos
- Architecture, deployment, and operational documentation
- Notes and references that apply across monitoring solutions
- Repository-wide documentation and standards

### `reports/`
- Monitoring reports and dashboard exports
- Performance summaries and insights
- Historical data and trend analyses
- Generated reports from various monitoring tools

### `solutions/`
- Product-specific documentation and configurations
- Deployment guides and setup instructions
- Templates, dashboards, and custom configurations
- Troubleshooting guides specific to each monitoring solution

## Naming Conventions

To maintain CLI-friendly filenames and consistent organization:

### File Naming Standards
- **Use lowercase kebab-case**: `my-document.md`, `netdata-config.yaml`
- **No spaces or uppercase**: Avoid `My Document.md` or `NETDATA_CONFIG.yaml`
- **Use appropriate extensions**: `.md` for documentation, `.yaml`/`.yml` for configs
- **Date format**: Use `YYYY-MM-DD` format for dated files (e.g., `report-2025-08-13.pdf`)

### Examples
✅ **Good**:
- `installation-guide.md`
- `netdata-insights-2025-08-13.pdf`
- `zabbix-host-templates.xml`
- `checkmk-bakery-config.yaml`

❌ **Avoid**:
- `Installation Guide.md`
- `Netdata Insights 8_13_25.pdf`
- `ZABBIX_HOST_TEMPLATES.XML`

## Per-Directory Indexes

Each solution directory should maintain its own documentation:

- [`solutions/netdata/README.md`](../solutions/netdata/) - Netdata-specific guides and configs
- [`solutions/zabbix/README.md`](../solutions/zabbix/) - Zabbix templates and procedures  
- [`solutions/checkmk/README.md`](../solutions/checkmk/) - CheckMK site configurations

## Contributing

When adding new content:

1. **Choose the right directory** based on scope (general docs vs. solution-specific)
2. **Follow naming conventions** to ensure CLI-friendly filenames
3. **Update relevant README files** to link to your new documentation
4. **Include brief descriptions** in directory indexes for discoverability

## Quick Navigation

- [General Documentation](.) - Repository-wide guides and standards
- [Monitoring Reports](../reports/) - Generated reports and exports
- [Solution Configurations](../solutions/) - Product-specific documentation
