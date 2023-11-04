<!-- BEGIN_TF_DOCS -->
{
  "header": "",
  "footer": "",
  "inputs": [
    {
      "name": "project_id",
      "type": "string",
      "description": "GCP project id",
      "default": null,
      "required": true
    },
    {
      "name": "region",
      "type": "string",
      "description": "The region for subnet",
      "default": null,
      "required": true
    },
    {
      "name": "subnet_cidr",
      "type": "string",
      "description": "CIDR range for subnet",
      "default": null,
      "required": true
    },
    {
      "name": "subnetwork_name",
      "type": "string",
      "description": "The name of the subnetwork",
      "default": null,
      "required": true
    },
    {
      "name": "vpc_name",
      "type": "string",
      "description": "The name of the VPC network",
      "default": null,
      "required": true
    }
  ],
  "modules": [],
  "outputs": [
    {
      "name": "network",
      "description": "vpc name"
    },
    {
      "name": "subnet",
      "description": "ubnet name"
    }
  ],
  "providers": [
    {
      "name": "google",
      "alias": null,
      "version": "5.4.0"
    }
  ],
  "requirements": [
    {
      "name": "terraform",
      "version": "\u003e= 0.13"
    }
  ],
  "resources": [
    {
      "type": "compute_network",
      "name": "default",
      "provider": "google",
      "source": "hashicorp/google",
      "mode": "managed",
      "version": "latest",
      "description": null
    },
    {
      "type": "compute_subnetwork",
      "name": "default",
      "provider": "google",
      "source": "hashicorp/google",
      "mode": "managed",
      "version": "latest",
      "description": null
    }
  ]
}
<!-- END_TF_DOCS -->    