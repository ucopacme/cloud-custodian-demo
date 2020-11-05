# Cloud Custodian Demo

### Install Cloud Custodian in a python virtual environment

```
brew install pipenv
pipenv install --python 3
pipenv shell
```

### Cloud Custodian Ops

#### Policy validation

```
custodian validate cloud-custodian/policies/cost-savings.yml
2020-11-05 09:05:34,510: custodian.commands:INFO Configuration valid: cloud-custodian/policies/ec2-offhours.yml
```

#### Policy dryrun

do a dry run of a policy and save output in /tmp/out

```
custodian run  --dryrun  -s /tmp/out  cloud-custodian/policies/cost-savings.yml
```
