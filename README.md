# K8SAPP: Kubernetes Application Template

[*Jump to quick start checklist, or ...*](#checklist)

*Replace the above title with your own.*

*Replace the description below with your own.*  

This GitHub template is meant to help encapsulate a Kubernetes
application consistent with the [K8SAPP Conventions][].

[K8SAPP Conventions]: https://github.com/rwxrob/k8sapp

## Application Repo Organization

*Remove the following paragraph after reading.*

> ⚠️  The term "application" here refers to everything within a specific
> Kubernetes namespace even though that namespace may contain several
> applications itself. You may wish to separate out applications within
> the same namespace depending on your situation. Consider carefully if
> your namespace contains multiple applications in composition (app only
> exists as a dependent part of the whole) or aggregation (app lives on
> independently of the whole) relationship.

This repo follows the K8SAPP conventions:

* `README.md` - description, notes, and references
* `k8sapp.yaml` - metadata about this application
* `check` - simple script to return 1 if update needed

## Application Management Procedures

*Remove this comment after documenting how to fetch, review, config,
install, update, uninstall, and check your namespaced application.*

Avoid putting any of this into a separate script (except `check`) since
things might change upon update and every change needs to be reviewed
again and *all* the management procedures could potentially need to be
updated.

### Fetching the Code

*Add explanation describing how to get the code safely in an
air-gapped environment.*

### Reviewing Code and Container Images

*Add explanation describing how the code was reviewed "by hand" and
should be in the future. Describe how the images should be retrieved in
an air-gapped environment and then scanned for vulnerabilities before
explaining how to push them to the internal container image registry.*

### Customizing and Configuring

*Add full description and instructions about how to customize the
default source code and configuration "by hand" to be compatible with
your internal cluster configuration and policies. Include code examples.
Consider flattening Helm charts and Kustomize overlays resulting in a
single resource YAML file.*

### Installing

*Add instructions for installing preferably using nothing but `kubectl`
commands and a single YAML resource file. Be sure to include references
to dependencies and prerequisites.*

### Updating

*Add instructions to update between each version of your configuration
(whether custom configuration or updates to the source itself).*

### Uninstalling

*Add instructions for how to cleanly uninstall everything related to
this namespaced application including any cluster-scoped resources
(RBAC, ClusterRole, etc.)*

### Check for Updates

*Add precise instructions for how to check for original source updates.
Strongly consider creating a `check` script that returns 1 if something
has changed and 0 if not. This allows update availability audits to be
automated.*

## Caveats

*Add warning, gotchas, and other special considerations to be aware of
for this specific namespaced Kubernetes application.*

## Relate References

*Add links to relevant sources and information.*

## Checklist

*Delete this section after using it to get started.*

- [ ] Change the title heading
- [ ] Update the description at the top of the README.md
- [ ] Decide whether to use a simple shell script or not (`k8sapp`)
- [ ] Fetch the code securely
- [ ] Document and/or automate the fetch process
- [ ] Review and understand the code, document caveats
- [ ] Add a namespace if needed 
- [ ] Make custom configurations as needed
- [ ] Document and/or automate configuration procedure
- [ ] Download, review, scan, and mirror container images
- [ ] Install the code locally and into dev and document installation
- [ ] Document and/or automate an upgrade procedure
- [ ] Document and/or automate an uninstall procedure
- [ ] Document and/or automate checking for updates 
- [ ] Document any additional references and URLs
- [ ] Add metadata to `k8sapp.yaml`
- [ ] Add an entry to the main `k8sapps` manifest meta repo 

