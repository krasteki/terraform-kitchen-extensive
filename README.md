### This repo contains terraform configuration which creates AWS resources. The purpose of it is to review the features of Kitchen-Terraform.

Following [this guide](https://newcontext-oss.github.io/kitchen-terraform/tutorials/extensive_kitchen_terraform.html)

git clone
cd

II. Generate SSH key
Mimic the following Bash script to generate an authentication key for SSH to be used by InSpec when authenticating with the AWS EC2 instances under test.
```
#!/bin/bash

# Make a directory to contain the key
mkdir -p test/assets

# Generate a 4096 bit RSA key with a blank passphrase in the directory
ssh-keygen \
  -b 4096 \
  -C "Kitchen-Terraform AWS provider tutorial" \
  -f test/assets/key_pair \
  -N "" \
  -t rsa
```

III. Create Test Fixture TF configuration

test/fixtures/wrapper/


IV. Create Terraform module





