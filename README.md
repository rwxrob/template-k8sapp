# Kubernetes Application Template (K8SAPP)

*Replace this description with your own.*  
[*Jump to quick start checklist.*](#checklist)

This GitHub template is meant to help encapsulate a Kubernetes
application consistent with the [K8SAPP Conventions][].

> ⚠️  The term "application" here refers to everything within a specific
> Kubernetes namespace even though that namespace may contain several
> applications itself. You may wish to separate out applications within
> the same namespace depending on your situation. Consider carefully if
> your namespace contains multiple applications in composition (app only
> exists as a dependent part of the whole) or aggregation (app lives on
> independently of the whole) relationship.

[K8SAPP Conventions]: https://github.com/rwxrob/k8sapp

## Use the `k8sapp` Shell Script

*Delete this section if creating a `k8sapp` or update to match your own
description.*

Although the K8SAPP conventions don't specify needing any additional
coding (only documented procedures) it is usually helpful to capture
these procedures as simple, well-documented, shell code. The
[`k8sapp`](k8sapp) script provides a simple starting shell script
template that includes minimal tab completion support.

## Checklist

- [ ] Change the title heading
- [ ] Update the description at the top of the README.md
- [ ] Decide whether to use a simple shell script or not (`k8sapp`)
- [ ] Fetch the code securely
- [ ] Document and/or automate the fetch process
- [ ] Review and understand the code, document caveats
- [ ] Configure the code
- [ ] Document and/or automate configuration procedure
- [ ] Add a namespace if needed 
- [ ] Install the code locally and into dev and document installation
- [ ] Document and/or automate an upgrade procedure
- [ ] Document and/or automate an uninstall procedure
- [ ] Document and/or automate checking for updates 
- [ ] Document any additional references and URLs
- [ ] Add metadata to `k8sapp.yaml`
- [ ] Add an entry to the main `k8sapps` manifest meta repo 
