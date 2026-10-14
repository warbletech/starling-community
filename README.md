# starling-community

Grok and Antigravity plugin for the public Starling Lite MCP.

**Endpoint:** <https://mcp.warbleoss.org/mcp> (`mode: readonly`)

The GitHub org `starling-ops` does not exist on this account. This repo is `warbletech/starling-community` until that org is created. The plugin name stays `starling-community`.

## Install

```bash
grok plugin install warbletech/starling-community --trust
```

Antigravity: add an MCP server with streamable HTTP URL `https://mcp.warbleoss.org/mcp`.

## What the model can call

Confirm with `tools/list`. As of the public demo:

- Cluster reads: `list_namespaces`, `list_pods`, `get_pod`, `get_pod_logs`, `list_nodes`, `list_events`, `list_deployments`, `list_hpas`, `list_pod_metrics`, `list_node_metrics`, `list_services`, `get_configmap`, `cluster_summary`
- Scans: `scan_manifest`, `scan_helm`, `scan_cluster_export`, `propose_remediation`

`scale_deployment`, `delete_pod`, and `apply_remediation` are not on this host.

Milestones: [MILESTONES.md](MILESTONES.md).

## License

Apache-2.0. See [LICENSE](LICENSE).
