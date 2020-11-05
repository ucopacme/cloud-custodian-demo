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
custodian validate cloud-custodian/policies/ec2-offhours.yml
2020-11-05 09:05:34,510: custodian.commands:INFO Configuration valid: cloud-custodian/policies/ec2-offhours.yml
```
