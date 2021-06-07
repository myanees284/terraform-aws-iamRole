# Terraform IAM role module
This terraform module creates the required IAM role.
## Usage
~~~
module "awsRole" {
  source      = "github.com/myanees284/tf-module-iamRole"
  policyFilePath = "policyfilefolder/inlinepolicies.json"
  iamRoleName = "your iam role name"
}
~~~