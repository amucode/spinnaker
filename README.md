# spinnaker-halyard
Ansible role for installing and configuring Spinnaker Using Halyard on AWS

# awscli 
Ansible role for installing and configuring awscli AWS

#### Prerequisite

- Platform: Ubuntu 14.04 
- Cloud Provider: kubernetes
- Ansible Version: 2.6.0
- Python Version: 2.7.15
- Kubectl Version: 1.10.1
- Spinnaker Version  1.8.0 and above

#### Default Vars - spinnaker-halyard

| Vars                                      | Description                              |
| :---------------------------------------  | :--------------------------------------- |
| spinnaker_halyard_installation_script_url | URL for downloading halyard              |
| spinnaker_version                         | Version of Spinnaker                     |
| cluster_name                              | Name of Kubernetes Cluster               |
| aws_access_key                            | AWS User MFA key                         |
| aws_secret_key                            | AWS User MFA Secret                      |
| aws_region                                | AWS region to create s3 bucket           |
| s3_bucket                                 | Provide Name for s3 bucket               | 
| kubectl_url                               | URL for downloading kubectl binary       |
| kubeconfig_file                           | Name of config file for kubernetes       |
| kubeconfig_source                         | hostmachine path to copy kube config file|
| kubeconfig_remote                         | Remote address to copy kube config file  |
| service_account                           | kubernetes service account               |
| namespaces                                | custom K8s namespaces to spinnaker       |
| docker_registry_name                      | Userdefined ECR name to spinnaker        | 
| docker_username                           | Bydefault in ECR it is AWS               |
| docker_registry_address                   | ECR registry address                     |
| docker_repositories                       | custom repository to bind with spinnaker |
| docker_login_token                        | token to login ECR                       |
| spinnaker_deck_url                        | Expose public URL to spinnaker UI        | 
| spinnaker_api_url                         | EXpose public URL to Spiinaker API       |
| jenkins_master_name                       | Userdefined Jenkins name to spinnaker    |
| jenkins_base_url                          | Remote Jenkins URL                       |
| jenkins_username                          | Remote Jenkins User                      |
| jenkins_user_token                        | Remote Jenkins User's API Token          |
------------------------------------------    ------------------------------------------

#### Vars - awscli

| Vars                                      | Description                              |
| :---------------------------------------  | :--------------------------------------- |
| aws_region                                | AWS default region                       |
| aws_output_format                         | AWS default poutput format               |
| aws_access_key                            | AWS User MFA key                         |
| aws_secret_key                            | AWS User MFA Secret                      |
------------------------------------------    ------------------------------------------


