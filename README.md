# Terraform IAM role module
This terraform module creates the required IAM role. The below 2 files must be present in current folder.<br><br>
policyFilePath - policy json file which will be attached to the role<br>
assumeRolePolicyName - trust relationship json file<br>
## Usage
~~~
module "awsRole" {
  source               = "github.com/myanees284/terraform-aws-iamRole"
  policyFilePath       = "policy file name.json"
  assumeRolePolicyName = "assume role.json"
  iamRoleName          = "some role name"
}
~~~
