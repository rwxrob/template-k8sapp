# Kubernetes Application Template

This GitHub template is meant to start (or encapsulate an existing)
Kubernetes application in a way that is minimally consistent and
supports the idea of separation of concerns with one application per git
repo (unlike the monorepo approach which provides no benefit in this
case).

* Every K8S app repo must have a `README.md` describing how to do the
  following (and preferably an `kapp` executable that supports these
  actions with tab completion):

  * Validate (`kapp validate`)
  * Install (`kapp install`)
  * Upgrade (`kapp upgrade`)
  * Uninstall (`kapp uninstall`)

Installing K8S applications seems to fall into one of the following
approaches (which are roughly ordered by level of complexity):

* Shell (`kubectl apply`)
* Kustomize
* Helm
* Modified Helm
* Operator Framework
* Custom Operators
