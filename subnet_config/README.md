# Azure - Kubernetes Module - Subnet Config

## Introduction

This sub-module configures subnets for use with AKS.
<br />

<!--- BEGIN_TF_DOCS --->
## Providers

| Name | Version |
|------|---------|
| azurerm | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:-----:|
| configure\_network\_role | Add Netowrk Contributor Role for subnet to AKS service principal. | `bool` | n/a | yes |
| configure\_nsg\_rules | Configure subnet NSG rules for AKS. | `bool` | n/a | yes |
| nsg\_rule\_priority\_start | Starting point for NSG rulee priorities. | `number` | n/a | yes |
| principal\_id | Id of principal which manages AKS | `string` | n/a | yes |
| subnet\_info | Azure virtual network subnet id. | `map(string)` | n/a | yes |

## Outputs

No output.
<!--- END_TF_DOCS --->
