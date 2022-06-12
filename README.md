# yc-s3-bucket

This project contains code for creating `yandex cloud s3 bucket` with `terraform`. 

---

## Usage

copy example and set your variables
```
cp terraform.tfvars.example terraform.tfvars
```
| Name                         | Description                                                                | Example                                  |
| ---------------------------- | -------------------------------------------------------------------------- | ---------------------------------------- |
| yc_token                     | https://cloud.yandex.ru/docs/iam/concepts/authorization/oauth-token        | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA  |
| yc_cloud_id                  | https://cloud.yandex.ru/docs/resource-manager/operations/cloud/switch-cloud| b1gg8sgd16g7qch5onqs                     |
| yc_folder_id                 | https://cloud.yandex.ru/docs/resource-manager/operations/folder/get-id     | b1gd129pp9ha0vnvf5g7                     |
| sa_name                      | service account name                                                       | tf-bucket-sa                             |

for running 
```bash
terraform init
terraform plan
terraform apply -auto-approve
```

for destroying
```bash
terraform destroy -auto-approve
```

---
## Installation

* terraform - [https://learn.hashicorp.com/tutorials/terraform/install-cli](https://learn.hashicorp.com/tutorials/terraform/install-cli).
* yandex.cloud provider - [https://registry.terraform.io/providers/yandex-cloud/yandex/latest/docs](https://registry.terraform.io/providers/yandex-cloud/yandex/latest/docs).
* yandex cli - [https://cloud.yandex.ru/docs/cli/operations/install-cli](https://cloud.yandex.ru/docs/cli/operations/install-cli).

## License
[MIT](https://choosealicense.com/licenses/mit/)