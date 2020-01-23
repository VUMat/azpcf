# azpcf
Concourse pipeline for deploying PCF on Azure


#TODO
- ~~opsman auth~~
- ~~configure Bosh director~~
- ~~deploy Bosh director~~
- ~~download stemcell and product (PAS)~~
- upload stemcell and product (PAS)
- configure product (PAS)
- deploy PAS
- download stemcell and product (PKS)
- upload stemcell and product (PKS)
- configure product (PKS)
- deploy PKS

setup credhub values from terraform output(to restore env):

director:
- bosh_storage_account_name
- azure_ssh_key.private_key/public
- set dns in dns provider

pas:
