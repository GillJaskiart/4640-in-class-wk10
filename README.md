# 4640-in-class-wk10

# Creating the key
`ssh-keygen -t ed25519 -f ~/.ssh/aws -C "lelechelsie@gmail.com"`

# Importing the key
`./scripts/import_lab_key ~/.ssh/aws.pub`

2. terraform
`terraform init` initialize directory and downloads plugins

`terraform fmt` to nicely format

`terraform validate` to validate the syntax

`terraform plan -out first_plan` create the plan and writes to file 'first_plan'

`terraform apply` to apply the configuration


**Outputs:**
>frontend = "44.248.30.21"
>redis = "52.88.212.42"

# Ansible Commands
3. Ansible
`ansible-playbook playbook.yml --syntax-check` to check the playbook

`ansible-playbook playbook.yml --check` to see what would change, similar to `terraform plan` without actually making any change.

`ansible-playbook playbook.yml` to run the playbook. Has to be run from inside the `/ansible` directory