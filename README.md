# Kubernetes Application Template (K8SAPP)

[*Jump to quick start checklist.*](#checklist)

This GitHub template is meant to start (or encapsulate an existing)
Kubernetes application consistent with the [K8SAPP Conventions][] in
a way that is minimally consistent and supports the idea of separation
of concerns with one application per git repo. This has the added
benefit of working well with a GitOps approach to deployment and
management.

> ⚠️  The term "application" here refers to everything within a specific
> Kubernetes namespace even though that namespace may contain several
> applications itself. You may wish to separate out applications within
> the same namespace depending on your situation. Consider carefully if
> your namespace contains multiple applications in composition (app only
> exists as a dependent part of the whole) or aggregation (app lives on
> independently of the whole) relationship.

[K8SAPP Conventions]: https://github.com/rwxrob/k8sapp

## Using a Simple `k8sapp` Shell Script



## Checklist

- [ ] Add a description of the in the first few paragraphs
- [ ] Add a section describing how to "
