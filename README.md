# azpcf
Concourse pipeline for deploying PCF on Azure


#TODO
- ~~opsman auth~~
- ~~configure Bosh director~~
- ~~deploy Bosh director~~
- ~~download stemcell and product (PAS)~~
- ~~upload stemcell and product (PAS)~~
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
- client_secret?

pas:



./pivnet login --api-token
ssh -i .ssh/azpcf_opsman ubuntu@pcf.pcfaz.matsukevich.altoros.com
wget https://github.com/pivotal-cf/pivnet-cli/releases/download/v1.0.0/pivnet-linux-amd64-1.0.0
chmod +x pivnet*
mv pivnet* pivnet
./pivnet download-product-files --product-slug='elastic-runtime' --release-version='2.8.2' --product-file-id=580787
wget https://github.com/pivotal-cf/om/releases/download/4.4.1/om-linux-4.4.1.tar.gz
 tar -xvf om-linux*
 create env.yml
 ./om --env env.yml upload-product -p srt-2.8.2-build.11.pivotal