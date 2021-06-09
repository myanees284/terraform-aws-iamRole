# Terraform IAM role module
This terraform module creates the required IAM role. The below 2 files must be present in current folder
policyFilePath - policy json file which will be attached to the role
assumeRolePolicyName - trust relationship json file
## Usage
~~~
module "awsRole" {
  source               = "github.com/myanees284/tf-module-iamRole"
  policyFilePath       = "policy file name.json"
  assumeRolePolicyName = "assume role.json"
  iamRoleName          = "some role name"
}
~~~