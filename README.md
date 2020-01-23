# azpcf
Concourse pipeline for deploying PCF on Azure


#TODO
- opsman auth
- configure Bosh director
- deploy Bosh director
- export installation
- upload stemcell and product (PAS)
- configure product (PAS)
- deploy PAS

setup credhub values from terraform output:
bosh_storage_account_name
azure_ssh_key.private_key/public
set dns in dns provider