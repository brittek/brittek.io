# Traffic Snapshots

This directory stores timestamped JSON snapshots of GitHub traffic metrics (views, clones, referrers, and popular paths) captured by the `traffic-snapshot` workflow.

Each file is named using the UTC timestamp of collection and the metric, for example:

```
2024-05-08T02-00-00Z-views.json
2024-05-08T02-00-00Z-clones.json
2024-05-08T02-00-00Z-popular-referrers.json
2024-05-08T02-00-00Z-popular-paths.json
```

> **Note:** The workflow requires a personal access token with `repo` and `traffic` scopes stored as `TRAFFIC_PAT` in the repository secrets. Without this secret the snapshot job will be skipped.
