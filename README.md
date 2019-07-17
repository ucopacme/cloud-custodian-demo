# Cloud Custodian Demo

### Install Prerequisites

```
brew install terraform
```

### Install Cloud Custodian

```
python3 -m venv custodian
source custodian/bin/activate
pip install c7n
```

### Create Demo AWS Environment

```
cd terraform
terraform init
terraform apply --auto-approve
```

### Run Cloud Custodian

```
custodian run -r eu-west-1 -s custodian/logs -m aws custodian-scheduled-availability-policy.yml
c7n-mailer --config custodian-slack-notification-policy.yml --update-lambda
```
