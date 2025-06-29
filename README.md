# Custom Krew Index

This is a custom plugin index for [Krew (kubectl plugin manager)](https://krew.sigs.k8s.io/).

## Available Plugins

| Plugin | Description | Repository |
|--------|-------------|------------|
| `image` | Manage container images in Kubernetes resources | [kubectl-image](https://github.com/reedchan7/kubectl-image) |

## Usage

### Add this index

```bash
kubectl krew index add reedchan7 https://github.com/reedchan7/krew-index.git
```

### Install plugins

```bash
# Install a specific plugin
kubectl krew install reedchan7/image

# Search available plugins
kubectl krew search reedchan7/
```

### List installed plugins

```bash
kubectl plugin list
```

### Upgrade plugins

```bash
kubectl krew upgrade reedchan7/image
```

### Remove this index

```bash
kubectl krew index remove reedchan7
```

## Supported Platforms

All plugins in this index support:
- macOS (Intel & Apple Silicon)
- Linux (AMD64 & ARM64) 
- Windows (AMD64)
