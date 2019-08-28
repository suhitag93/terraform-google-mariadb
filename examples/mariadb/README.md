# Simple Example

This example illustrates running the terraform script to build a mariadb cluster with high availability on Compute Engine instances.
=======
This example illustrates how to use the `mariadb` module.


<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Inputs
We need to set variables for terraform to allocate the appropriate resources on google cloud.




| Name        | Description                   | Type  | Default | Required  |
|-------------|-------------------------------|:-----:|:-----:|:-----------:|
| bucket_name | Name of the bucket to create. | string| n/a   | yes |
| project_id  | ID of the project to provision resources. | string  | n/a | yes |
| cluster_name|Name of created cluster.       |string |n/a    | yes |
| vm_image    | password for rootuser access | string | n/a | yes |
| garb_instance_type| password for rootuser access | string | n/a  | yes |
| garb_zone   | Galera artibtrator zone | string  | n/a|yes |
| garb_region | Galera artibtrator region | string |n/a  | yes |
| garb_subnetwork | Galera artibtrator subnetwork | string | n/a | yes |
| network_project |password for rootuser access | string  | yes |
| network     |password for rootuser access | string | n/a | yes |
| service_account | | string |
| instance_type |
| client_ip_range |
| pass      | password for rootuser access | string  | yes |
| replpass  |     | string  | yes |
| statspass |     | string  | yes |
| disk_size_gb |    | string  | yes |
| disk_type | ssd or standard    | string | yes
| health_check_name | Name of healthcheck |


## Outputs

| Name | Description |
|------|-------------|
| bucket\_name | The name of the bucket. |

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

To provision this example, run the following from within this directory:
- `terraform init` to get the plugins
- `terraform plan` to see the infrastructure plan
- `terraform apply` to apply the infrastructure build
- `terraform destroy` to destroy the built infrastructure
