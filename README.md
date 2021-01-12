KernelCI Tekton Experiments
===========================

This repository contains early experiments using [Tekton](https://tekton.dev/)
with the aim to implement a Cloud-native KernelCI pipeline.

Proof of concept
----------------

KernelCI already relies on Kubernetes to build Linux kernels with GCE and Azure
clusters.  We're now investigating how we can use the full potential of this
technology in order to run other kinds of payloads and come up with a more
scalable design than the current Jenkins pipeline.

Initially as a proof-of-concept, the first objectives are to:

* get familiar with Tekton and Kubernetes to better understand what can be done
* determine whether Tekton appears to be a suitable tool for KernelCI's use-case
* identify any weaknesses that might prevent us from using it in production

This may be done by creating a basic version of the current pipeline used in
production (building kernels, submitting tests...) or by running other
experiments to see how individual features can be used.
