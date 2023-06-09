# curvefs-csi

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.0](https://img.shields.io/badge/AppVersion-1.0.0-informational?style=flat-square)

A Helm chart for CurveFs CSI Driver

**Homepage:** <https://github.com/opencurve/curvefs-csi>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| h0hmj | <h0hmjcn@gmail.com> |  |

## Source Code

* <https://github.com/opencurve/curvefs-csi>

## Requirements

Kubernetes: `>=1.18.0-0`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| controller.nodeSelector | object | `{}` |  |
| controller.resources.limits.cpu | string | `"1000m"` |  |
| controller.resources.limits.memory | string | `"1Gi"` |  |
| controller.resources.requests.cpu | string | `"100m"` |  |
| controller.resources.requests.memory | string | `"512Mi"` |  |
| driver.name | string | `"csi.curvefs.com"` |  |
| driver.repository | string | `"harbor.cloud.netease.com/curve/curvefs"` |  |
| driver.tag | string | `"csi-v1.0.0"` |  |
| kubeletDir | string | `"/var/lib/kubelet"` |  |
| node.hostNetwork | bool | `false` |  |
| node.nodeSelector | object | `{}` |  |
| node.resources.limits.cpu | string | `"4000m"` |  |
| node.resources.limits.memory | string | `"4Gi"` |  |
| node.resources.requests.cpu | string | `"100m"` |  |
| node.resources.requests.memory | string | `"512Mi"` |  |
| sidecars.csiProvisionerImage.repository | string | `"quay.io/k8scsi/csi-provisioner"` |  |
| sidecars.csiProvisionerImage.tag | string | `"v1.6.0"` |  |
| sidecars.nodeDriverRegistrarImage.repository | string | `"quay.io/k8scsi/csi-node-driver-registrar"` |  |
| sidecars.nodeDriverRegistrarImage.tag | string | `"v1.3.0"` |  |
| storageClass.allowVolumeExpansion | bool | `false` |  |
| storageClass.enabled | bool | `true` |  |
| storageClass.mountOptions | string | `nil` |  |
| storageClass.name | string | `"curvefs-cs"` |  |
| storageClass.parameters.fsType | string | `"s3"` |  |
| storageClass.parameters.mdsAddr | string | `""` |  |
| storageClass.parameters.s3AccessKey | string | `""` |  |
| storageClass.parameters.s3Bucket | string | `""` |  |
| storageClass.parameters.s3Endpoint | string | `""` |  |
| storageClass.parameters.s3SecretKey | string | `""` |  |
| storageClass.reclaimPolicy | string | `"Delete"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
