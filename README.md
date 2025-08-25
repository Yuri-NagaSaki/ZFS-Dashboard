# ZFS Grafana Dashboard

A comprehensive monitoring dashboard for ZFS storage systems, designed to work with the [ZFS Exporter](https://github.com/pdf/zfs_exporter) v2.3.10.

## Dashboard Features

### Pool Health Monitoring
- **Health Status**: Real-time pool condition (ONLINE/DEGRADED/FAULTED)
- **Capacity Metrics**: Total size, allocated space, and available storage
- **Fragmentation Level**: Pool fragmentation percentage tracking
- **Deduplication Ratio**: Space savings through data deduplication
- **Read-Only Status**: Pool accessibility monitoring

### Storage Analytics
- **Usage Visualization**: Pie charts and gauges for space utilization
- **Trend Analysis**: Historical view of storage consumption patterns
- **Dataset Breakdown**: Individual filesystem space usage tracking
- **Capacity Planning**: Long-term storage growth insights

## Data Sources

The dashboard utilizes metrics exposed by the [ZFS Exporter](https://github.com/pdf/zfs_exporter), which interfaces with ZFS through standard system commands and exports data in Prometheus format.

### Key Metrics
- `zfs_pool_size_bytes` - Total pool capacity
- `zfs_pool_allocated_bytes` - Used storage space
- `zfs_pool_free_bytes` - Available storage space
- `zfs_pool_fragmentation_ratio` - Pool fragmentation level
- `zfs_pool_deduplication_ratio` - Deduplication efficiency
- `zfs_dataset_used_bytes` - Per-dataset space consumption


For detailed implementation information, refer to the [ZFS Exporter project](https://github.com/pdf/zfs_exporter).
