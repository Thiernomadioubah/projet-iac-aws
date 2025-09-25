## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_instance.web_server](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |
| [aws_security_group.web_sg](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_ami_id"></a> [ami\_id](#input\_ami\_id) | L'ID de l'AMI à utiliser pour l'instance EC2. | `string` | n/a | yes |
| <a name="input_environment_tag"></a> [environment\_tag](#input\_environment\_tag) | Tag d'environnement. | `string` | n/a | yes |
| <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type) | Le type d'instance EC2. | `string` | `"t2.micro"` | no |
| <a name="input_project_name"></a> [project\_name](#input\_project\_name) | Nom du projet pour les tags. | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_instance_id"></a> [instance\_id](#output\_instance\_id) | L'ID de l'instance EC2 créée. |
| <a name="output_public_ip"></a> [public\_ip](#output\_public\_ip) | L'adresse IP publique de l'instance EC2 créée. |
| <a name="output_security_group_id"></a> [security\_group\_id](#output\_security\_group\_id) | L'ID du groupe de sécurité créé. |
