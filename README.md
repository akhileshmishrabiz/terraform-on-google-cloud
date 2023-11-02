<!-- BEGIN_TF_DOCS -->
## Requirements

The following requirements are needed by this module:

- <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) (>= 0.13)

## Providers

The following providers are used by this module:

- <a name="provider_google"></a> [google](#provider\_google) (5.4.0)

## Modules

No modules.

## Resources

The following resources are used by this module:

- [google_compute_network.default](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_network) (resource)
- [google_compute_subnetwork.default](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/compute_subnetwork) (resource)

## Required Inputs

The following input variables are required:

### <a name="input_project_id"></a> [project\_id](#input\_project\_id)

Description: GCP project id

Type: `string`

### <a name="input_region"></a> [region](#input\_region)

Description: The region for subnet

Type: `string`

### <a name="input_subnet_cidr"></a> [subnet\_cidr](#input\_subnet\_cidr)

Description: CIDR range for subnet

Type: `string`

### <a name="input_subnetwork_name"></a> [subnetwork\_name](#input\_subnetwork\_name)

Description: The name of the subnetwork

Type: `string`

### <a name="input_vpc_name"></a> [vpc\_name](#input\_vpc\_name)

Description: The name of the VPC network

Type: `string`

## Optional Inputs

No optional inputs.

## Outputs

The following outputs are exported:

### <a name="output_network"></a> [network](#output\_network)

Description: vpc name

### <a name="output_subnet"></a> [subnet](#output\_subnet)

Description: ubnet name
<!-- END_TF_DOCS -->    