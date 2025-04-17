# geekoops-prometheus-node_exporter

Enable and configure the prometheus node_exporter for exposing prometheus stats from any system.

## Role Variables

| Variable | Default | Description |
|----------|---------|-------------|
| `prometheus_node_exporter_args` | '' | Additional arguments for `node_exporter` to run. |

# Example Playbook

```
- hosts: jellyfish
  roles:
      - role: geekoops-prometheus-node_exporter
        vars:
          prometheus_node_exporter_args: '--collector.systemd'
```