kubectl plugin that scans the images of a kubernetes resource using Trivy container image scanner ([https://github.com/aquasecurity/trivy](https://github.com/aquasecurity/trivy))

# Usage

```
kubectl trivy <kubernetes-resource>
```

Where `<kubernetes-resource>` is anything that `kubectl get` support.
Examples:

```
kubectl trivy pod mypod
kubectl trivy pod mypod -n mynamespace
kubectl trivy pods
kubectl trivy pods -n mynamespace
kubectl trivy deployment mydeployment
kubectl trivy job myjob
```

# Install

Download the file `kubectl-trivy` to somewhere on your path

## Requirements

1. Trivy
1. bash
1. sed

