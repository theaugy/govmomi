[![Build](https://github.com/vmware/govmomi/actions/workflows/govmomi-go-build.yaml/badge.svg)](https://github.com/vmware/govmomi/actions/workflows/govmomi-go-build.yaml)
[![Test](https://github.com/vmware/govmomi/actions/workflows/govmomi-go-test.yaml/badge.svg)](https://github.com/vmware/govmomi/actions/workflows/govmomi-go-test.yaml)
[![Go Report Card](https://goreportcard.com/badge/github.com/vmware/govmomi)](https://goreportcard.com/report/github.com/vmware/govmomi)
[![Latest Release](https://img.shields.io/github/release/vmware/govmomi.svg?logo=github&style=flat-square)](https://github.com/vmware/govmomi/releases/latest)
[![Go Reference](https://pkg.go.dev/badge/github.com/vmware/govmomi.svg)](https://pkg.go.dev/github.com/vmware/govmomi)
[![go.mod Go version](https://img.shields.io/github/go-mod/go-version/vmware/govmomi)](https://github.com/vmware/govmomi)

# govmomi

A Go library for interacting with VMware vSphere APIs (ESXi and/or vCenter).

In addition to the vSphere API client, this repository includes:

* [govc](./govc) - vSphere CLI

* [vcsim](./vcsim) - vSphere API mock framework

* [toolbox](./toolbox) - VM guest tools framework

## Compatibility

This library is built for and tested against ESXi and vCenter 6.5, 6.7 and 7.0.

It may work with versions 5.1, 5.5 and 6.0, but neither are officially supported.

## Documentation

The APIs exposed by this library very closely follow the API described in the [VMware vSphere API Reference Documentation][apiref].
Refer to this document to become familiar with the upstream API.

The code in the `govmomi` package is a wrapper for the code that is generated from the vSphere API description.
It primarily provides convenience functions for working with the vSphere API.
See [godoc.org][godoc] for documentation.

[apiref]:https://code.vmware.com/apis/968/vsphere
[godoc]:http://godoc.org/github.com/vmware/govmomi

## Installation

```sh
go get -u github.com/vmware/govmomi
```

## Discussion

Contributors and users are encouraged to collaborate using GitHub issues and/or
[Slack](https://vmwarecode.slack.com/messages/govmomi).
Access to Slack requires a [VMware {code} membership](https://code.vmware.com/join/).

## Status

Changes to the API are subject to [semantic versioning](http://semver.org).

Refer to the [CHANGELOG](CHANGELOG.md) for version to version changes.

## Projects using govmomi

* [Docker Machine](https://github.com/docker/machine/tree/master/drivers/vmwarevsphere)

* [Docker InfraKit](https://github.com/docker/infrakit/tree/master/pkg/provider/vsphere)

* [Docker LinuxKit](https://github.com/linuxkit/linuxkit/tree/master/src/cmd/linuxkit)

* [Kubernetes](https://github.com/kubernetes/kubernetes/tree/master/pkg/cloudprovider/providers/vsphere)

* [Kubernetes Cloud Provider](https://github.com/kubernetes/cloud-provider-vsphere)

* [Kubernetes Cluster API](https://github.com/kubernetes-sigs/cluster-api-provider-vsphere)

* [Kubernetes kops](https://github.com/kubernetes/kops/tree/master/upup/pkg/fi/cloudup/vsphere)

* [Terraform](https://github.com/terraform-providers/terraform-provider-vsphere)

* [Packer](https://github.com/jetbrains-infra/packer-builder-vsphere)

* [VMware VIC Engine](https://github.com/vmware/vic)

* [Travis CI](https://github.com/travis-ci/jupiter-brain)

* [collectd-vsphere](https://github.com/travis-ci/collectd-vsphere)

* [Gru](https://github.com/dnaeon/gru)

* [Libretto](https://github.com/apcera/libretto/tree/master/virtualmachine/vsphere)

* [Telegraf](https://github.com/influxdata/telegraf/tree/master/plugins/inputs/vsphere)

* [Open Storage](https://github.com/libopenstorage/openstorage/tree/master/pkg/storageops/vsphere)

* [Juju](https://github.com/juju/juju)

* [vSphere 7.0](https://docs.vmware.com/en/VMware-vSphere/7.0/rn/vsphere-esxi-vcenter-server-7-vsphere-with-kubernetes-release-notes.html)

* [OPS](https://github.com/nanovms/ops)

* [VMware Event Broker Appliance](https://github.com/vmware-samples/vcenter-event-broker-appliance/tree/development/vmware-event-router)

## Related projects

* [rbvmomi](https://github.com/vmware/rbvmomi)

* [pyvmomi](https://github.com/vmware/pyvmomi)

* [go-vmware-nsxt](https://github.com/vmware/go-vmware-nsxt)

## License

govmomi is available under the [Apache 2 license](LICENSE.txt).

## Name

Pronounced "go-v-mom-ie"

Follows pyvmomi and rbvmomi: language prefix + the vSphere acronym "VM Object Management Infrastructure".
