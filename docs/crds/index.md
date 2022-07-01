# Overview

This project houses CustomResourceDefinitions (CRDs) related to security and compliance checks along with the code
generated by Kubernetes [code generators][k8s-code-generator] to write such custom resources in a programmable way.

| NAME                          | SHORTNAMES                | APIGROUP               | NAMESPACED | KIND                                                                 |
|-------------------------------|------------------------------|------------------------|------------|----------------------------------------------------------------------|
| [vulnerabilityreports]        | vulns,vuln                   | aquasecurity.github.io | true       | [VulnerabilityReport](./vulnerability-report.md)                     |
| [configauditreports]          | configaudit,configaudits     | aquasecurity.github.io | true       | [ConfigAuditReport](./configaudit-report.md)                         |
| [exposedsecretsreports]       | exposedsecret,exposedsecrets | aquasecurity.github.io | true       | [ExposedSecretReport](./exposedsecret-report.md)               |



[k8s-code-generator]: https://github.com/kubernetes/code-generator

[vulnerabilityreports]: https://raw.githubusercontent.com/aquasecurity/trivy-operator/{{ git.tag }}/deploy/crd/vulnerabilityreports.crd.yaml
[configauditreports]: https://raw.githubusercontent.com/aquasecurity/trivy-operator/{{ git.tag }}/deploy/crd/configauditreports.crd.yaml
[exposedsecretsreports]: https://raw.githubusercontent.com/aquasecurity/trivy-operator/{{ git.tag }}/deploy/crd/exposedsecrets.crd.yaml