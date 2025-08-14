# Monitoring Reports

This directory contains monitoring reports, dashboard exports, and performance analyses from various monitoring tools.

## Current Reports

### Netdata Reports
- [`netdata-insights-7d-summary-2025-08-13-all-nodes.pdf`](./netdata-insights-7d-summary-2025-08-13-all-nodes.pdf) - 7-day infrastructure summary for all monitored nodes

## Report Categories

### Performance Reports
- System performance summaries and trend analyses
- Resource utilization reports and capacity planning
- Network performance and connectivity reports

### Health Reports
- Infrastructure health assessments
- Service availability and uptime reports
- Alert and incident summary reports

### Compliance & Audit Reports
- Security monitoring and compliance reports
- Configuration drift and audit trail reports
- Backup and disaster recovery status reports

## Naming Conventions

Follow these patterns for consistent, CLI-friendly report naming:

### Format Pattern
`{tool}-{report-type}-{time-period}-{date}-{scope}.{ext}`

### Examples
- `netdata-insights-7d-summary-2025-08-13-all-nodes.pdf`
- `zabbix-availability-monthly-2025-08-web-servers.pdf`
- `checkmk-performance-weekly-2025-08-15-database-cluster.html`

### Components
- **tool**: `netdata`, `zabbix`, `checkmk`, etc.
- **report-type**: `insights`, `availability`, `performance`, `security`, etc.
- **time-period**: `daily`, `weekly`, `monthly`, `7d`, `30d`, etc.
- **date**: `YYYY-MM-DD` format
- **scope**: `all-nodes`, `web-servers`, `database-cluster`, etc.
- **extension**: `.pdf`, `.html`, `.csv`, `.json`, etc.

## Automated Reports

### Schedule & Retention
- **Daily Reports**: Kept for 30 days
- **Weekly Reports**: Kept for 6 months  
- **Monthly Reports**: Kept for 2 years
- **Quarterly Reports**: Kept indefinitely

### Report Sources
- **Netdata Cloud**: Automated exports from Netdata insights
- **Zabbix Frontend**: Dashboard exports and custom reports
- **CheckMK**: WATO reports and custom analytics
- **Custom Scripts**: Automated report generation tools

## Related Documentation

- [General Documentation](../docs/) - Repository-wide guides
- [Solution Configurations](../solutions/) - Tool-specific setup and configs
- [Netdata Solutions](../solutions/netdata/) - Netdata-specific documentation
- [Zabbix Solutions](../solutions/zabbix/) - Zabbix-specific documentation
- [CheckMK Solutions](../solutions/checkmk/) - CheckMK-specific documentation

## Contributing

When adding new reports:
- Follow the [naming conventions](#naming-conventions) above
- Update this index with new report descriptions
- Include brief summaries of report contents
- Archive old reports according to retention policies
